# Resumo do lab - Microsoft Azure Essentials

## 1. Microsoft Azure - Localizando Serviços por Categoria
* A aula é destinada à apresentação da plataforma Azure, pontuando alguns detalhes como configurações pessoais do portal, como aparência e idioma, além da apresentação da aba "Serviços", onde podemos visualizar todos os serviços disponíveis na plataforma, organizados por categorias
  
## 2. Criando máquinas Virtuais na Azure
* Aula que aborda principalmente a questão do SLA(Service Level Agreement) que representa uma especie de acordo assumido com a Azure, em geral, o tempo máximo que determinado serviço pode ficar indisponivel, tendo limites semanais, mensais e anuais. Esse acordo varia de acordo com diversos fatores, entre elas, as zonas de disponibilidade, ou a quantidade de máquinas que tivermos
* Quanto maior o nível de SLA em %, menor será o tempo tolerado das falhas. EX : 99% - 1,68 hora / 99,9% - 10,1 minutos

## 3. Configurando uma instância de Banco de Dados na Azure
* Aula que apresenta uma breve amostra das configurações ao criar uma instancia de vm ou banco de dados, destacando a parte do preview sobre os custos que teremos utilizando determinada configuração

## 4. Construindo Arquiteturas no Azure
* Aula que inicia sobre a questão dos datacenters e zonas de disponibilidade, onde podemos encontrar a lista de datacenters
* Segunda parte ensinando sobre a criaçao de um Grupo de recursos e alguns atalhos que temos, além da criação de uma rede privada

## 5. Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure
* Aula que aborda sobre o tema de dimensionamento em máquinas virtuais, inicialmente a criaçao de uma máquina virtual e seus diferentes tipos e configurações, sistemas operacionais
* Logo em seguida, é mostrado a parte da configuração do dimensionamento, possibilitando configurarmos diferentes configurações como CPU e RAM aumentadas para determinados horarios de pico ou stress
* Tipos de armazenamento de disco, algumas métricas e configurações como desligamento automatico, backup e etc

## 6. Dominando o Armazenamento na Azure
* Tipos de armazenamento azure, Blob Storage para armazenamento não estruturado de arquivos, imagens, vídeos e backups, Azure Files serviços da azure que permite o compartilhamento de arquivos gerenciados, Disk Storage para máquinas virtuais, otimizados para desempenho e confiabilidade, Table Storage para armazenamento de tabelas noSQL e Queue Storage para armazenamento de filas
* Parte de redundancia : LRS (Locally Redundant Storage): Três cópias dos dados dentro do mesmo datacenter, oferecendo alta durabilidade local. ZRS (Zone-Redundant Storage): Armazenamento redundante em várias zonas de disponibilidade dentro de uma região, proporcionando proteção contra falhas de datacenter. GRS (Geo-Redundant Storage) e RA-GRS (Read-Access Geo-Redundant Storage): Replicação dos dados entre regiões geograficamente distantes para garantir alta disponibilidade e recuperação em caso de falhas regionais
* AzCopy: Ferramenta de linha de comando para copiar dados de e para contas de armazenamento no Azure de forma rápida e eficiente
* Azure Storage Explorer: Interface gráfica para gerenciar contas de armazenamento, permitindo visualizar, criar, copiar, mover e excluir arquivos e objetos com facilidade

## 7. Entendendo sobre Segurança e Identidade na Azure
* Microsoft Defender for Cloud  para fornecer visibilidade em tempo real das ameaças e vulnerabilidades, ajudando a gerenciar a postura de segurança dos recursos
* Azure Active Directory (Azure AD) é o serviço central de identidade e autenticação no Azure, permitindo a gerência centralizada de usuários, grupos e permissões
* NSGs (Network Security Groups) para controlar o tráfego de entrada e saída das redes virtuais e proteger os recursos contra acessos não autorizados
* A Azure fornece criptografia automática para dados em trânsito e em repouso para garantir a segurança das informações armazenadas e transferidas
* Uso de ferramentas como o Azure Monitor e o Azure Sentinel (SIEM) para acompanhar eventos e detectar atividades suspeitas, permitindo respostas rápidas a incidentes de segurança

## 8. Otimizando Custos no Azure
* Azure Cost Management para monitorar e analisar o uso e os custos associados aos recursos em tempo real, permitindo que os usuários acompanhem seus gastos e identifiquem picos de consumo
* Configuração de alertas de orçamento e dashboards personalizados para notificar quando os custos ou o uso se aproximarem de limites predefinidos, ajudando a prevenir surpresas no faturamento
* Escolher tamanho de VM e RAM de acordo com a necessidade, evitando custos desnecessarios, configuração do auto-scaling para adicionar ou remover recursos automaticamente conforme a demanda, garantindo que você pague apenas pelo que utiliza. e desligar os recursos que não estiverem em uso via script ou automações
* Azure Reservations: Aquisição de instâncias reservadas para VMs e outros serviços com descontos significativos (até 72%) em comparação com o pagamento sob demanda
* Azure Hybrid Benefit: Uso de licenças locais existentes de Windows Server e SQL Server para reduzir custos ao migrar para o Azure, aproveitando a infraestrutura já licenciada
* Instâncias Spot: Utilização de VMs de baixo custo (spot) para workloads que são tolerantes a interrupções, permitindo economias significativas

## 9. Gerenciando Politicas em Acessos Azure
* Azure Policy permite criar, gerenciar e aplicar políticas que garantem que os recursos estejam em conformidade com regras organizacionais ou requisitos de conformidade, como padrões de segurança, tipos de VMs permitidos ou configurações de rede específicas
* A política é atribuída a um escopo, que pode ser um grupo de gerenciamento, uma assinatura, um grupo de recursos ou um recurso específico
* O RBAC (Role-Based Access Control) é usado para gerenciar quem tem acesso a recursos específicos e quais ações podem ser realizadas, seguindo o princípio de menor privilégio e permite a atribuição de funções predefinidas ou personalizadas a usuários, grupos ou identidades de serviço, como Owner(Controle total sobre o recurso, incluindo a gestão de acesso), Colaborador (Permissão para gerenciar recursos, mas sem alterar configurações de acesso) e Leitor(Acesso apenas para visualizar informações sem possibilidade de modificar)
* Azure AD é o serviço central para gerenciar identidades e permissões na plataforma Azure, integrando com RBAC para autenticação e autorização
* Azure Monitor e Azure Security Center ajudam a monitorar e auditar os acessos e conformidade das políticas, fornecendo alertas e relatórios quando há desvios ou tentativas de acessos não autorizados

## 10. Ferramentas de Implantação na Azure
* Azure Portal é a interface gráfica baseada na web usada para criar, configurar e gerenciar recursos manualmente é bom para implantações rápidas ou experimentações, mas pode não ser eficiente para cenários de escala ou repetição, pois depende de interações manuais
* Azure CLI e Azure PowerShell são ferramentas de linha de comando que permitem automação e gerenciamento de recursos diretamente do terminal são úteis para escrever scripts e automatizar processos, facilitando a execução de implantações repetitivas e complexas de forma eficiente
* Os ARM Templates utilizam arquivos JSON para descrever de forma declarativa a infraestrutura e a configuração de serviços do Azure e permitem implantações consistentes e repetitivas, possibilitando a automação e o controle de versão dos recursos, ideal para cenários de infraestrutura como código (IaC) úteis para provisionamento em larga escala e para garantir a conformidade e padronização de configurações
* Azure DevOps é uma plataforma que integra ferramentas de integração contínua/entrega contínua (CI/CD), gerando pipelines automatizados para o desenvolvimento, teste e implantação de aplicações e infraestrutura, permite a criação de pipelines de build e release, automatizando processos como teste de código, criação de pacotes e deploy em ambientes de desenvolvimento, homologação ou produção
* GitHub Actions pode ser integrado com o Azure para configurar pipelines de CI/CD diretamente do GitHub, gerenciando desde o controle de versão até a implantação automatizada dos recursos e aplicações e é ideal para desenvolvedores que utilizam o GitHub como repositório principal, facilitando a integração com o Azure e a automação de fluxos de trabalho
* Terraform é uma ferramenta open-source que permite a provisionamento e gerenciamento de infraestrutura em múltiplas nuvens utilizando uma linguagem declarativa, usado para criar e gerenciar recursos de forma consistente e automatizada, com suporte para controle de versão e reutilização de configurações, sendo amplamente utilizado em ambientes híbridos e multicloud
* O Azure Bicep é uma linguagem simplificada que facilita a criação de templates para a implantação de recursos no Azure, sendo uma alternativa mais simples e legível em comparação aos ARM Templates tradicionais, melhorando a experiência de infraestrutura como código, oferecendo sintaxe mais limpa e suporte nativo ao Azure, tornando o gerenciamento e a automação de infraestrutura mais eficientes
* Azure Kubernetes Service (AKS) é utilizado para orquestrar contêineres no Azure, facilitando a implantação e o gerenciamento de aplicações baseadas em contêineres em escala
* Helm permite a criação de charts para configurar e gerenciar a implantação de contêineres e suas dependências de forma simplificada e reutilizável

## 11. Monitoramento Inteligente com o Azure
* O Azure Monitor é a principal ferramenta de monitoramento do Azure, que coleta telemetria e logs de recursos na nuvem e ambientes locais, como VMs, redes, bancos de dados e aplicativos, proporcionando uma visão unificada e centralizada do desempenho e da integridade dos recursos, facilitando a identificação de problemas e a tomada de decisões baseadas em dados
* Monitoramento de infraestrutura como máquinas virtuais (VMs), redes e contêineres, com métricas que incluem uso de CPU, memória, latência de rede e outros indicadores críticos
* Criação de dashboards personalizados no Azure Monitor para consolidar métricas e logs importantes em uma única interface, facilitando a visualização e o acompanhamento em tempo real
* Configuração de ações automáticas em resposta a alertas, como escalonamento de recursos, execução de scripts ou notificações via e-mail/SMS para equipes de operações
* Monitoramento de ameaças de segurança em conjunto com o Microsoft Defender for Cloud, que analisa logs e eventos de segurança para detectar atividades suspeitas
