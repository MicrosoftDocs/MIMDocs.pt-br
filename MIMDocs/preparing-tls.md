---
title: Planejar o Microsoft Identity Manager 2016 no ambiente TLS 1.2 | Microsoft Docs
description: Planejar o Microsoft Identity Manager 2016 no ambiente TLS 1.2
keywords: ''
author: billmath
ms.author: billmath
manager: daveba
ms.date: 10/26/2017
ms.topic: conceptual
ms.prod: microsoft-identity-manager
ms.assetid: 50345fda-56d7-4b6e-a861-f49ff90a8376
ms.reviewer: mwahl
ms.suite: ems
ms.openlocfilehash: 4e208e2f42c206ae50febefb6a8206dc3823e084
ms.sourcegitcommit: c9f5f960fd39745bf5b57161a2fd0238c88d035a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133525"
---
# <a name="planning-mim-2016-sp2-in-tls-12-or-fips-mode-environments"></a>Planejar o MIM 2016 SP2 em ambientes de modo TLS 1.2 ou FIPS


> [!IMPORTANT]
> Este artigo se aplica somente ao MIM 2016 SP2

Ao instalar o MIM 2016 SP2 no ambiente bloqueado que tem todos os protocolos de criptografia, mas o TLS 1.2 desabilitado, os seguintes requisitos se aplicam:
- Para estabelecer uma conexão segura TLS 1.2, os componentes MIM necessitam das atualizações mais recentes do Windows Server e do .NET Framework que permitem a instalação do suporte ao TLS 1.2 no .NET 3.5 Framework. Dependendo da configuração do servidor, *pode* ser necessário [habilitar o SystemDefaultTlsVersions para .NET Framework](https://support.microsoft.com/help/3154520/support-for-tls-system-default-versions-included-in-the-net-framework) e/ou [desabilitar todos os protocolos SCHANNEL, exceto o TLS 1.2](https://docs.microsoft.com/windows-server/security/tls/tls-registry-settings) no registro nas subchaves *Client* e *Server*.

## <a name="mim-synchronization-service-sql-ma"></a>Serviço de Sincronização do MIM, SQL MA

- Para estabelecer uma conexão TLS 1.2 segura com o SQL Server, o Serviço de Sincronização do MIM e o agente de gerenciamento do SQL interno requerem o [SQL Native Client 11.0.7001.0](https://www.microsoft.com/download/details.aspx?id=50402) ou posterior.

## <a name="mim-service"></a>Serviço MIM
   >[!NOTE]
   >A instalação autônoma do MIM 2016 SP2 falha em ambientes que têm apenas o TLS 1.2. Instale o Serviço do MIM no modo interativo ou, se estiver instalando de modo autônomo, verifique se o TLS 1.1 está habilitado. Após a conclusão da instalação autônoma, aplique o TLS 1.2, se necessário.

- Os certificados autoassinados não podem ser usados pelo serviço do MIM no ambiente somente TLS 1.2. Escolha um certificado compatível com criptografia forte emitido pela Autoridade de Certificação confiável ao instalar o Serviço do MIM.
- O instalador do serviço do MIM também precisa do [Driver do OLE DB para SQL Server versão 18.2](https://www.microsoft.com/download/details.aspx?id=56730) ou posterior.

## <a name="fips-mode-considerations"></a>Considerações sobre o modo FIPS

Se você instalar o serviço do MIM em um servidor com o modo FIPS habilitado, será necessário desabilitar a validação da política FIPS para permitir que os Fluxos de Trabalho de Serviço do MIM sejam executados. Para fazer isso, adicione o elemento *enforceFIPSPolicy enabled=false* à seção *runtime* do arquivo *Microsoft.ResourceManagement.Service.exe.config* entre as seções *runtime* e *assemblyBinding*, conforme mostrado abaixo:

```XML
<runtime>
<enforceFIPSPolicy enabled="false"/>
<assemblyBinding ...>
```    
