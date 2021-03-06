# [Compreender e explorar](../microsoft-identity-manager-2016.md)
## [O que é o MIM 2016?](../microsoft-identity-manager-2016.md)
### [Scripts de implantação do MIM2016 SP1 PAM](../sp1-deployment-scripts.md)
## [Saiba mais sobre o PAM](../pam/privileged-identity-management-for-active-directory-domain-services.md)
## [Relatório híbrido no Azure](../identity-manager-hybrid-reporting-azure.md)
# [Planejar e projetar](../microsoft-identity-manager-2016-supported-platforms.md)
## [Plataformas com suporte](../microsoft-identity-manager-2016-supported-platforms.md)
## [Conectar aos diretórios](../supported-management-agents.md)
## [Planejamento de capacidade](../capacity-planning-guide.md)
## [Topologia de implantação](../topology-considerations.md)
## [Planejar a implantação do PAM](../pam/environment-overview.md)
# [Implantação e usar](../microsoft-identity-manager-deploy.md)
## [Implantação inicial](../microsoft-identity-manager-deploy.md)
### [Configuração de domínio](../preparing-domain.md)
### [Configuração de servidor: Windows Server](../prepare-server-ws2016.md)
### [Configuração de servidor: SQL](../prepare-server-sql2016.md)
### [Configuração de servidor: SharePoint](../prepare-server-sharepoint.md)
### [Configuração de servidor: Exchange](../prepare-server-exchange.md)
### [Instalação do MIM: sincronização](../install-mim-sync.md)
### [Instalação do MIM: serviço e portal](../install-mim-service-portal.md)
### [Instalação do MIM: sincronizar bancos de dados](../install-mim-sync-ad-service.md)
## [Atualizar do Forefront Identity Manager 2010 R2](../microsoft-identity-manager-2016-upgrade-from-fim-2010-R2.md)
## [Instalar o MIM Certificate Management](../mim-cm-deploy.md)
## [Tópicos sobre a instalação do BHOLD](../bhold/bhold-installation-guide.md)
### [Instalação do módulo BHOLD Core](../bhold/bhold-core-installation.md)
### [Instalação do módulo Integração do BHOLD](../bhold/bhold-integration-installation.md)
### [Instalação do módulo Atestado do BHOLD](../bhold/bhold-attestation-installation.md)
### [Instalação do módulo Gerador de modelos do BHOLD](../bhold/bhold-model-generator-installation.md)
### [Instalação do módulo Relatórios do BHOLD](../bhold/bhold-reporting-installation.md)
### [Instalação do módulo Análise do BHOLD](../bhold/bhold-analytics-installation.md)
### [Instalação do módulo Conector de gerenciamento de acesso do BHOLD](../bhold/bhold-access-management-connector-install.md)
## [Serviço de Notificação de Alteração de Senha](../deploying-mim-password-change-notification-service-on-domain-controller.md)
## [Relatório Híbrido do Identity Manager](../working-with-identity-manager-hybrid-reporting.md)
## [Autoatendimento de Redefinição de Senha](../working-with-self-service-password-reset.md)
## [Gerenciador de Certificados do MIM](../working-with-mim-certificate-manager.md)
### [Registrar cartões inteligentes](../certificate-manager-for-non-administrators.md)
### [Criação de certificados de software](../certificate-manager-for-software-certificates.md)
# [Usar o Privileged Access Management](../pam/privileged-identity-management-for-active-directory-domain-services.md)
## [Configurar o MIM para o Privileged Access Management](../pam/configuring-mim-environment-for-pam.md)
## [Noções básicas sobre os componentes](../pam/principles-of-operation.md)
### [Visão geral do ambiente](../pam/environment-overview.md)
### [Modelo de camada](../pam/tier-model-for-partitioning-administrative-privileges.md)
### [Planejar um ambiente de bastiões](../pam/planning-bastion-environment.md)
### [Definir funções](../pam/defining-roles-for-pam.md)
### [Alta disponibilidade e recuperação de desastre](../pam/high-availability-disaster-recovery-considerations-bastion-environment.md)
### [Requisitos de hardware e software](../pam/hardware-software-requirements.md)
### [Etapa 1 – Domínio CORP](../pam/step-1-prepare-corp-domain.md)
### [Etapa 2 – Controlador de domínio PRIV](../pam/step-2-prepare-priv-domain-controller.md)
### [Etapa 3 – Servidor PAM](../pam/step-3-prepare-pam-server.md)
### [Etapa 4 – Instalar o MIM no servidor PAM](../pam/step-4-install-mim-components-on-pam-server.md)
### [Etapa 5 – Estabelecer a relação de confiança entre PRIV e CORP](../pam/step-5-establish-trust-between-priv-corp-forests.md)
### [Etapa 6 – Criar contas privilegiadas](../pam/step-6-transition-group-to-pam.md)
### [Etapa 7 – elevar o acesso do usuário](../pam/step-7-elevate-user-access.md)
### [Implantar o PAM do MIM com o Windows Server 2016](../pam/deploy-pam-with-windows-server-2016.md)
### [Configurar o Azure MFA](../pam/use-azure-mfa-for-activation.md)
## [Configurar o PAM usando scripts](../pam/sp1-pam-configure-using-scripts.md)
### [Etapa 1 Configurando o domínio Priv](../pam/sp1-step1-configuring-priv-domain.md)
### [Etapa 2 Configurando o domínio CORP](../pam/sp1-step2-configuring-corp-domain.md)
### [Etapa 3 Configurar o SQL](../pam/sp1-step3-installing-configuring-sql.md)
### [Etapa 4 Configurar o SharePoint](../pam/sp1-step4-configuring-sharepoint.md)
### [Etapa 5 Instalar/configurar o PAM](../pam/sp1-step5-configuring-pam.md)
### [Etapa 6 Configurar a relação de confiança do PAM](../pam/sp1-step6-setup-pam-trust.md)
### [Etapa 7 Configurar o histórico de SID/filtragem de SID](../pam/sp1-step7-setup-sidhistory-sidfiltering.md)
### [Etapa 8 Verificação de implantação do PAM](../pam/sp1-step8-pam-deployment-verification.md)
### [Adendo](../pam/sp1-pam-deployment-addendum.md)
# Gerenciar a Infraestrutura
## [Analisador de práticas Recomendadas para o Gerenciador de Identidades](https://technet.microsoft.com/library/jj203402)
## [Serviço de Notificação de Alteração de Senha](https://technet.microsoft.com/library/e27c0bc6-c808-4fdb-9e59-58feeb419308)
## Gerenciamento de certificado
### [Ferramenta de Linha de Comando CLMUtil](https://technet.microsoft.com/library/cc720647)
### [Modelos de Perfil de Configuração](https://technet.microsoft.com/library/cc708656)
### [Usando o site de gerenciamento de certificado](https://technet.microsoft.com/library/cc720560)
### [Gerenciamento de Aplicativos de Cartão Inteligente](https://technet.microsoft.com/library/cc708681)
### [Backup e Restauração](https://technet.microsoft.com/library/dd883245)
## Autoatendimento de Redefinição de Senha
### [Registro do Usuário de Programação](https://technet.microsoft.com/library/jj134294)
### [Personalizações do Portal](../reference/mim-portal-customizations.md)
## Serviço e Portal
### [Kerberos](https://technet.microsoft.com/library/jj134299)
### [Registro dinâmico](mim-service-dynamic-logging.md)
### [Guia de Desempenho de Exportação](https://technet.microsoft.com/library/hh322883)
## Relatórios
### [Relatando Relatórios Personalizados e Extensibilidade](https://technet.microsoft.com/library/jj133861)
# [Referência](../reference/microsoft-identity-manager-2016-developer-reference.md)
## Referência do desenvolvedor
### [Referência do MIM 2016 para desenvolvedores](../reference/microsoft-identity-manager-2016-developer-reference.md)
### BHOLD
#### [Referência do BHOLD para desenvolvedores](../reference/mim2016-bhold-developer-reference.md) 
### [Referência da API REST do Certificate Manager](../reference/certificate-management-rest-api-reference.md)
#### [Detalhes do serviço da API REST do CM](../reference/certificate-management-rest-api-service-details.md)
#### [Instruções passo a passo de registro de exemplo](../reference/sample-enrollment-walkthrough.md)
#### [Obter modelos de perfil](../reference/get-profile-templates.md)
#### [Operações da política](../reference/policy-operations.md)
#### [Obter a política de fluxo de trabalho](../reference/get-workflow-policy.md)
#### [Obter a política de cartão inteligente](../reference/get-smartcard-policy.md)
#### [Operações de solicitação](../reference/request-operations.md)
##### [Criar solicitação](../reference/create-request.md)
##### [Obter solicitação](../reference/get-request.md)
##### [Cancelar, abandonar ou concluir uma solicitação](../reference/cancel-abandon-complete-request.md)
#### [Operações de solicitação de certificado](../reference/certificate-request-operations.md)
##### [Obter opções de geração de solicitação de certificado](../reference/get-certificate-request-generation-options.md)
##### [Obter respostas de certificado](../reference/get-certificate-responses.md)
#### [Operações de cartão inteligente](../reference/smartcard-operations.md)
##### [Atribuir cartão inteligente a uma solicitação](../reference/assign-smartcard-to-request.md)
##### [Obter dados de cartão inteligente](../reference/get-smartcard-data.md)
##### [Obter resposta de autenticação de cartão inteligente](../reference/get-smartcard-authentication-response.md)
##### [Obter chave de administração diversificada de cartão inteligente](../reference/get-smartcard-diversified-admin-key.md)
##### [Obter o PIN proposto do cartão inteligente](../reference/get-smartcard-proposed-pin.md)
##### [Atualizar o status do cartão inteligente](../reference/update-smartcard-status.md)
#### [Operações do perfil](../reference/profile-operations.md)
##### [Obter dados do perfil](../reference/get-profile-data.md)
##### [Obter operações de estado do perfil](../reference/get-profile-state-operations.md)
#### [Operações de certificado](../reference/certificate-operations.md)
##### [Obter certificados de perfil ou cartão inteligente](../reference/get-smartcard-profile-certificates.md)
##### [Obter certificados do usuário](../reference/get-user-certificates.md)
### [Referência da API REST do PAM (Gerenciamento de Acesso Privilegiado)](../reference/privileged-access-management-rest-api-reference.md)
#### [Detalhes do serviço da API REST do PAM](../reference/privileged-access-management-rest-api-service-details.md)
#### [Obter funções do PAM](../reference/privileged-access-management-get-roles.md)
#### [Criar solicitação do PAM](../reference/privileged-access-management-create-request.md)
#### [Obter solicitações do PAM](../reference/privileged-access-management-get-requests.md)
#### [Encerrar solicitação do PAM](../reference/privileged-access-management-close-request.md)
#### [Obter solicitações do PAM pendentes](../reference/privileged-access-management-get-pending-requests.md)
#### [Aprovar ou rejeitar uma solicitação pendente do PAM](../reference/privileged-access-management-approve-reject-pending-request.md)
#### [Obter informações de sessão do PAM](../reference/privileged-access-management-get-session-info.md)
## Referência técnica
### [Terminologia do Microsoft Identity Manager 2016 SP1](../reference/mim-2016-sp1-terms.md)
### [Referência do XML de Configuração de Exibição de Controle de Recurso](../reference/rcd-configuration-xml-reference.md)
### [Códigos de erro de Execução do Agente de Gerenciamento](../reference/maerrorcodes.md)
### [Referência de função para Microsoft Identity Manager 2016](../reference/mim2016-functions-reference.md)
### [Referência do Gerenciamento de Senhas para Microsoft Identity Manager 2016](mim2016-password-management.md)
### BHOLD
#### [Guia de conceitos do BHOLD](../bhold/bhold-concepts-guide.md)
## Histórico de versão
### [Histórico de versão do MIM](../reference/version-history.md)
### [Histórico de versão do BHOLD](../reference/version-bhold-history.md)
