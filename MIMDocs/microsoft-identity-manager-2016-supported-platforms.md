---
title: Plataformas de software com suporte | Microsoft Docs
description: "Localize os produtos e versões compatíveis com cada um dos componentes do MIM 2016"
keywords: 
author: billmath
ms.author: billmath
manager: femila
ms.date: 03/28/2017
ms.topic: article
ms.service: microsoft-identity-manager
ms.technology: security
ms.assetid: 4978f60d-044d-4e84-8d93-65801fce1144
ms.reviewer: mwahl
ms.suite: ems
translationtype: Human Translation
ms.sourcegitcommit: f1faed3a09023e288a68a8950dae43725f19eb3e
ms.openlocfilehash: 33c84afa4d6fd2ed7bde33de39dd151f83f07fd4
ms.lasthandoff: 04/12/2017


---

# <a name="supported-platforms-for-mim-2016"></a>Plataformas com suporte para o MIM 2016

Esta tabela descreve as plataformas com suporte, e a versão de cada componente do Microsoft Identity Manager 2016. As versões marcadas com um * só têm suporte no MIM 2016 service pack 1.


| **Componente do MIM** | **Plataforma** | **Versão** |
|-------------------|--------------|-------------|
| **Sincronização do MIM** | Windows Server | Windows Server 2008 R2 SP1<br/>Windows Server 2012<br/>Windows Server 2012 R2<br/>Windows Server 2016 * |
| | Banco de dados da Sincronização do MIM | SQL Server 2008 R2 SP3<br/>SQL Server 2012 SP2<br/>SQL Server 2014 SP1 <br/> SQL Server 2016 * |
| | Active Directory para provisionamento de usuário, PCNS e Sincronização GAL (opcional)|Windows Server 2008 R2 SP1<br/>Windows Server 2012<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Exchange para provisionamento de caixa de correio e Sincronização GAL (opcional)|Exchange Server 2010 SP3<br/>Exchange Server 2013 SP1<br/>Exchange Server 2016* |
| | Ambiente de desenvolvimento (opcional) | Visual Studio 2012<br/>Visual Studio 2013 <br/> Visual Studio 2015 <br/> Visual Studio 2017* |
| | Sistema conectado adicional (opcional) | Active Directory Domain Services<br/>Active Directory<br/>Lightweight Directory Services<br/>SQL Server 2000 ou posterior<br/>SharePoint Server 2013<br/> SharePoint Server 2016 * <br/> Outros produtos de terceiros |
| **Serviço do MIM** (exceto cenário de PAM) | Windows Server | Windows Server 2008 R2 SP1<br/>Windows Server 2012<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Banco de dados do Serviço do MIM | SQL Server 2008 R2 SP3<br/>SQL Server 2012 SP2<br/>SQL Server 2014 SP1 <br/> SQL Server 2016 * |
| | Exchange para aprovação do Serviço do MIM e emails de gerenciamento de grupo (opcional) | Exchange Server 2010 SP3<br/>Exchange Server 2013 SP1 <br/> Exchange Server 2016 * <br/> Exchange Online * (Somente Notificação) |
| **Serviço do MIM e Portal** (somente cenário de PAM)| Windows Server | Windows Server 2012<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Active Directory para a floresta do PAM no ambiente de bastiões | Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Active Directory para florestas existentes | Windows Server 2008 <br/> Windows Server 2008 R2 * <br/> Windows Server 2012 * <br/> Windows Server 2012 R2 * <br/> Windows Server 2016 * |
| | Banco de dados do Serviço do MIM | SQL Server 2008 R2 SP3<br/>SQL Server 2012 SP2<br/>SQL Server 2014 SP1 <br/> SQL Server 2016 * |
| | SharePoint | SharePoint Foundation 2010<br/>SharePoint Foundation 2013 SP1 <br/> SharePoint 2016 * |
| | Servidor de email para aprovação do Serviço do MIM e emails de gerenciamento de grupo (opcional) | Exchange Server 2010 SP3<br/>Exchange Server 2013 SP1 <br/> Exchange Server 2016 * <br/> Exchange Online * (Somente Notificação) |
| | Navegador | Todos os principais navegadores |
| **Relatórios do Serviço do MIM** | Windows Server | Windows Server 2012 <br/> Windows Server 2016 * |
| | Data Warehouse | System Center 2012 Service Manager <br/> System Center 2012 R2 Service Manager </br> System Center 2016 Service Manager * (Com 4.4.1459)<br/> [Compatibilidade de Versão do SQL Server para o System Center 2016](https://technet.microsoft.com/en-us/system-center-docs/system-requirements/sql-server-version-compatibility)
 |
| **Portais de Registro e Redefinição de Senha do MIM** | Windows Server | Windows Server 2008 R2 SP1<br/>Windows Server 2012<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Navegador da Web | Todos os principais navegadores |
| **Suplementos e extensões do MIM** | Windows | Windows 7<br/>Windows 8<br/>Windows 8.1<br/>Windows 10 |
| | Integração com o Outlook (opcional) | Outlook 2007 SP2<br/>Outlook 2010<br/>Outlook 2013 <br/> Outlook 2016 (no Windows 10) * |
| | Cmdlets do solicitante do PowerShell no PAM (opcional) | Windows 8.1<br/>Windows 10 |
| **Gerenciamento de certificados do MIM** (Integração de servidor e a AC (Autoridade de Certificação)) | Windows server | Windows Server 2008 R2 SP1<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Autoridade de certificação | Windows Server 2008 R2 SP1<br/>Windows Server 2012<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Banco de dados do MIM CM | SQL Server 2008 R2 SP3<br/>SQL Server 2012 SP2<br/>SQL Server 2014 SP1 <br/> SQL Server 2016 * |
| **Gerenciamento de certificados do MIM** (Aplicativo) | Windows | Windows 8<br/>Windows 8.1<br/>Windows 10 |
| **Gerenciamento de certificados do MIM** (Cliente e cliente em massa) | Windows | Windows 7 |
| **Suite MIM BHOLD** | Windows Server | Windows Server 2008 R2 SP1<br/>Windows Server 2012 R2 <br/> Windows Server 2016 * |
| | Banco de dados BHOLD | SQL Server 2008 R2 SP3<br/>SQL Server 2012 SP2 <br/> SQL Server 2014 * <br/> SQL Server 2016 * |
| | Servidor de email (opcional) | Exchange Server 2010 SP3<br/>Exchange Server 2013 SP1 <br/> Exchange Server 2016 * |
| | Navegador da Web | Internet Explorer 7, 8, 9, 10 ou 11 com Silverlight |
