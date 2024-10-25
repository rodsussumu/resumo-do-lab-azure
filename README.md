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
* Parte de redundancia : LRS (Locally Redundant Storage): Três cópias dos dados dentro do mesmo datacenter, oferecendo alta durabilidade local. ZRS (Zone-Redundant Storage): Armazenamento redundante em várias zonas de disponibilidade dentro de uma região, proporcionando proteção contra falhas de datacenter. GRS (Geo-Redundant Storage) e RA-GRS (Read-Access Geo-Redundant Storage): Replicação dos dados entre regiões geograficamente distantes para garantir alta disponibilidade e recuperação em caso de falhas regionais.
* AzCopy: Ferramenta de linha de comando para copiar dados de e para contas de armazenamento no Azure de forma rápida e eficiente.
* Azure Storage Explorer: Interface gráfica para gerenciar contas de armazenamento, permitindo visualizar, criar, copiar, mover e excluir arquivos e objetos com facilidade
