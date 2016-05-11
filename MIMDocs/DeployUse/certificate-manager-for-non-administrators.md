---
# required metadata

title: Registrar cartões inteligentes para não administradores | Microsoft Identity Manager
description: Saiba como registrar cartões inteligentes para os computadores de usuários sem acesso de administrador para que possam usar o Gerenciador de certificados.
keywords:
author: kgremban
manager: stevenpo
ms.date: 04/28/2016
ms.topic: article
ms.prod: identity-manager-2015
ms.service: microsoft-identity-manager
ms.technology: security
ms.assetid: bfabc562-a2f0-4cff-ac31-36927f41e102

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: mwahl
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Registrar cartões inteligentes para não administradores
Se um usuário não for um administrador local no seu computador, ele não poderá registrar um cartão inteligente em seu próprio computador por padrão. O procedimento a seguir permite que você contorne essa limitação.

## Habilitando a renovação do cartão inteligente para não administradores no Gerenciador de certificados 2016 MIM

1.  **Descompactar o arquivo appx**

    Obter um certificado de assinatura. Siga as etapas para [Assinar aplicativos do Windows 8 usando uma PKI interna](http://blogs.technet.com/b/deploymentguys/archive/2013/06/14/signing-windows-8-applications-using-an-internal-pki.aspx). Pare quando chegar a "Assinar o aplicativo". Atribua um nome ao arquivo pfx exportado. Exporte para um arquivo .cer e importe para o cliente que esteja usando o arquivo cer do novo certificado de autenticação.

    Execute o seguinte para desempacotar o arquivo appx:

    `makeappx unpack /l /p <app package name>.appx /d ./appx`

    `ren <app package name>.appx <app package name>.appx.old`

    `cd appx`

2.  **Modificar o arquivo de configuração**

    Renomeie o arquivo chamado `CustomDataExample.xml custom.data`. O aplicativo CM procurará por este nome de arquivo.

    Edite o arquivo custom.data e modifique o seguinte:

    1.  No elemento &lt;NonAdmin&gt;, altere o valor do atributo Value para "Verdadeiro"

    2.  Salve o arquivo e saia do editor

    3.  Exclua o arquivo chamado AppxSignature.p7x

    4.  Edite o arquivo chamado AppxManifest.xml

    5.  No elemento <Identity>, modifique o valor do atributo Publisher para a entidade do certificado de autenticação, por exemplo "CN=ABCD"

        O assunto aqui deve ser o mesmo que o assunto no certificado de autenticação que você está usando para assinar o aplicativo.

    6.  Salve o arquivo e saia do editor.

3.  **Empacotar novamente e assinar o pacote do aplicativo (arquivo appx)**

    Execute o seguinte para empacotar e assinar o arquivo appx:

    `cd ..`

    `makeappx pack /l /d .\appx /p <app package name>.appx`

    s`igntool sign /f <path\>mysign.pfx /p <pfx password> /fd "sha256" <app package name>.appx`

4.  Duplique o modelo de perfil e adicione a chave de administrador inicial para configurar o servidor MIM:

    1.  Faça logon no portal do CM como um usuário com privilégios administrativos.

    2.  Acesse **Administração** &gt; **Gerenciar modelos de perfil** e certifique-se de que a caixa esteja marcada ao lado do modelo de perfil que você criou, então clique em Copiar um modelo de perfil selecionado.

    3.  Digite o nome do modelo de perfil, adicione "nonAdmin" e clique em **OK**.

    4.  Quando as configurações gerais do modelo de perfil forem exibidas, role para baixo totalmente e, em **Configuração do Cartão Inteligente**, clique em **Alterar Configurações**.

    5.  Em **Valor inicial da chave de administrador (hexadecimal)** , insira a chave de administrador padrão: "010203040506070801020304050607080102030405060708"

    6.  Role para baixo e clique em **OK**.

5.  **Crie uma conta não administrativa no computador cliente**

    Os usuários não administradores não podem criar o cartão inteligente virtual do TPM, você precisará criá-lo para eles.

6.  **Criar um cartão de inteligente virtual usando TpmVscMgr**

    Execute o seguinte (ainda como administrador) para criar um cartão inteligente virtual vazio em um computador. Isso pode ser feito por meio do Intune, o SCCM ou grupo de políticas.

    `TpmVscMgr create /name MyVSC /pin default /adminkey default /generate`

7.  **Instalar o aplicativo CM na conta de não administrativa**

8.  **Inicie o aplicativo CM e registre-se para um cartão inteligente virtual**


<!--HONumber=Apr16_HO2-->

