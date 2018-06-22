---
title: Idiomas com suporte no Microsoft Identity Manager 2016 SP1 | Microsoft Docs
description: Uma lista de idiomas com suporte no Microsoft Identity Manager 2016 SP1.
keywords: ''
author: fimguy
ms.author: davidste
manager: mbaldwin
ms.date: 05/23/2018
ms.topic: get-started-article
ms.service: microsoft-identity-manager
ms.technology: security
ms.assetid: 50345fda-56d7-4b6e-a861-f49ff90a8376
ms.openlocfilehash: 101f4110d6439cfc17f25c8880531e18f51920da
ms.sourcegitcommit: 19ed53fa6af61086774a0429fd1520067caf4e93
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2018
---
# <a name="supported-languages"></a>Idiomas com suporte

Este artigo descreve os idiomas com suporte e o mapeamento de atualizações do Microsoft Identity Manager 2016 SP1 versão 4.5.x ou superior.

## <a name="mim-service-and-portal-and-add-ins-and-extensions-language-pack"></a>Pacote de Idiomas de Extensões e Suplementos e Serviço e Portal do MIM 

O Pacote de Idiomas do Serviço e Portal do Microsoft MIM oferece suporte para os 33 idiomas a seguir.  

> [!NOTE]
> No [4.4.1642.0](https://support.microsoft.com/en-us/help/4021562/hotfix-rollup-package-build-4-4-1642-0-is-available-for-microsoft), foi adicionada uma chave de registro chamada "OverrideDefaultUILocale" ao pacote de idioma Extensões e Suplementos do MIM, que tentará mapear todos os idiomas semelhantes àquele que tem suporte. Por exemplo, se o idioma de exibição do Windows for ES-CL (espanhol do Chile) ou qualquer ES - **, ele tentará mapeá-lo para ES-ES (espanhol da Espanha).

> [!IMPORTANT]
> O texto no suplemento SSPR e no portal será localizado, mas as perguntas não serão feitas sem trabalho adicional. Você precisará criar fluxos de trabalho de AuthN (e conjuntos e MPRs acompanhantes para direcioná-los) para direcionar perguntas em cada idioma para o local de destino.

|Language|FIM(4.3.x.x)/MIM(4.4.xx)|MIM(4.5.x.x)
|-----|-----|-----|
|Búlgaro|bg-BG|bg|
|Chinês (simplificado)|zh-CN|zh-hans|
|Chinês (Taiwan)|zh-TW|zh-hant|
|Croata|hr-HR|hr|
|Tcheco|cs-CZ|cs|
|Dinamarquês|da-DK|da|
|Holandês|nl-NL|nl|
|Estoniano|et-EE|et|
|Francês|fr-FR|fr|
|Finlandês|fi-FI|fi|
|Alemão|de-DE|de|
|Grego|el-GR|el|
|Hindi|hi-IN|hi|
|Húngaro|hu-HU|hu|
|Italiano|it-IT|it|
|Japonês|ja-JP|ja|
|Coreano|ko-KR|ko|
|Lituano|lt-LT|lt|
|Letão|lv-LV|lv|
|Norueguês|nb-NO|nb-NO|
|Polonês|pl-PL|pl|
|Português (Portugal)|pt-PT|pt|
|Português (Brasil)|pt-BR|pt-BR|
|Russo|ru-RU|ru||sv|
|Romeno|ro-RO|ro|
|Espanhol|es-ES|Sim|
|Eslovaco|sk-SK|sk|
|Sueco|sv-SE|sv|
|Esloveno|sl-SI|sl|
|Sérvio - Sérvia |sr-latn-CS (obsoleto)|sr-Latn-RS|
|Tailandês|th-TH|th|
|Turco|tr-TR|tr|
|Ucraniano|uk-UA|uk|

## <a name="certificate-management"></a>Gerenciamento de certificado 
O Gerenciamento de Certificados da Microsoft oferece suporte aos 9 idiomas a seguir. 

|Language|FIM(4.3.x.x)/MIM(4.4.xx)|New MIM(4.5.x.x)
|-----|-----|-----|-----|
|Chinês (simplificado)|zh-CN|zh-hans|
|Chinês (Taiwan)|zh-TW|zh-hant|
|Holandês|nl-NL|nl|
|Francês|fr-FR|fr|
|Alemão|de-DE|de|
|Italiano|it-IT|it|
|Japonês|ja-JP|ja|
|Português (Portugal)|pt-PT|pt-PT|
|Espanhol|es-ES|Sim|

## <a name="certificate-management-modern-application"></a>Aplicativo Moderno de Gerenciamento de Certificados  
O Aplicativo Moderno de Gerenciamento de Certificados da Microsoft oferece suporte aos 33 idiomas a seguir. 

|Language | [1.0.225.104](https://www.microsoft.com/en-us/download/details.aspx?id=54954) | |
|-----|-----|-----|-----|
|Holandês|nl-NL|nl|
|Chinês (simplificado)|zh-CN|zh-hans|
|Chinês (Taiwan)|zh-TW|zh-hant|
|Tcheco|cs-CZ|cs|
|Dinamarquês|da-DK|da|
|Francês|fr-FR|fr|
|Finlandês|fi-FI|fi|
|Alemão|de-DE|de|
|Grego|el-GR|el|
|Húngaro|hu-HU|hu|
|Italiano|it-IT|it|
|Japonês|ja-JP|ja|
|Coreano|ko-KR|ko|
|Norueguês|nb-NO|nb-NO|
|Polonês|pl-PL|pl|
|Português (Portugal)|pt-PT|pt|
|Português (Brasil)|pt-BR|pt-BR|
|Russo|ru-RU|ru|
|Romeno|ro-RO|ro|
|Espanhol|es-ES|Sim|
|Sueco|sv-SE|sv|
|Turco|tr-TR|tr|

## <a name="next-steps"></a>Próximas etapas

- [Implantação inicial](microsoft-identity-manager-deploy.md)
- [Histórico de Versão](/reference/version-history.md)