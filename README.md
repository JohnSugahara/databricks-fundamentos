# Databricks e seus Fundamentos.

## Tópicos

### 1° Historia das plataformas de manejamento de dados.

### 2° O que é a Plataforma Databricks Intelligence?

### 3° Arquitetura da Plataforma Databricks DI e Fundamentais de Segurança.

*a.* Visão geral da arquitetura da plataforma.

*b.* Data governance.

*c.* Segurança, Confiabilidade e Performance.

*d.* The Data Intelligence Engine

### 4° Workloads suportadas na Plataforma Databricks DI

*a.* Data warehousing

*b.* Orchestration

*c.* ETL & analise tempo-real

*d.* Data science & AI

### 5° Sumário e Proximos passos.

---

## The History of Data Management Platforms.

### No fim dos anos 80(1980) empresas queriam possuir as percepções movidas por data(data-driven insights) para decisões empresariais e inovação. 

Para isso organizações precisavam sair dos dados coletados apenas por simples bases relacionais para sistemas que manejavam e analisavam data que estava sendo generada em tempo real e que coletaria grandes volumes em uma velocidade rapida.

<p align="center">
  <img src="images/datawarehouse.png" width="100">
</p>

Data Warehouse foram criadas para coletar e consolidar o fluxo de dados e prover suporte geral para dados de inteligencia e analise de empresas.

Data e Data Warehouses eram estruturadas e limpas, com esquemas pre-definidos.
Porém Data Warehouses nao foram feitas com datas meio estruturadas ou não estruturadas em mente, dessa forma não havia suporte para dados sem o padrão correto.

Isso causou inflexibilidade em esquematicos, problema com pico de volume e velocidade, e longo tempo de procesamento.

Com o avanço do mundo digital isso apenas piorou, por que dados aumetaram em volume, velocidade e variedade.

O que causou que desfavoreceu as Data Warehouses, tomava muito tempo para processsar dados e providenciar resultados. E tinha capacidade limitada para lidar com variedade de data e velocidade. 

### Em 2000 teve uma acensão de algo chamado **"Big Data"**, o que ocasionando a criação dos **Data Lake**s.

O Data Lake permitia que dados estruturados, semi estruturados e não estruturados conseguissem conviver no mesmo ambiente simultaneamente. Dados que eram coletados em volume e velocidade necessarios para dar suporte ao ritmo de geração de dados da epoca.  

<p align="center">
  <img src="images/datalake.png" width="100">
</p>

Diversos dados diferentes poderiam ser guardados lado a lado em um Data Lake, dados que eram criados de diferentes origens, sejam elas logs de web ou dados de sensores poderiam ser transmitidos para o Data Lake com facilidade, velocidade e de maneira barata em armazenamento de objetos cloud de preço baixo.

Apesar dos Data Lakes resolverem o problema de armazenamento eles criaram novos problemas, não possuiam coisas necessarias que Data Warehouses tinham.

Data Lakes nao tinham suporte para dados transacionais e não podiam reforçar qualidade de dados. Então não se tinha confiança nos dados dos Data Lakes.

Também pela alta quantidade de data a velocidade de analise era bem lenta, e a oportunidade de decisões de resultado com impacto nunca se manifestou.

E governancia de dados em um data lake cria desafios para o reforço de segurança e privacidade por causa da falta de estrutura dos dados de um data lake.

### Em 2021 a ascensão do paradigma da arquitetura LakeHouse ocorreu.

Em 2013 databricks foi fundada e em 2020 introduziu para o mundo a primeira e unica Plataforma Lakehouse em Cloud, combinando os melhores aspectos de Data Warehouses e Data Lakes em uma plataforma unificada e aberta para dados e IA.

Em 2021 os fundadores da Databricks e outros individuos cunharam o termo "Arquitetura Lakehouse" no artigo "Lakehouse: A nova geração de plataformas abertas que unificam Data Warehousing e Analise Avançada"

<p align="center">
  <img src="images/datalakehouse.png" width="100">
</p>

Times de empresas ficavam discronizados, usando tecnologias separadas Data Warehouses e Data Lakes causavam problemas de velocidade de entrega.

Para resolver esse problema Databricks matou a necessidade de algo unificado e simples criando o Data Lakehouse.

Combinando os beneficios de um data lake e o poder de analise e controle de um Data Warehouse. Isso criou uma fonta confiavel de dados, combinando acesso direto a IA e BI trabalharem juntos, com uma governancia de segurança unificada.

<p align="center">
  <img src="images/keydatalakehouse.png" width="100">
</p>

Agora empresas podiam guardar, refinar, analisar e acessar dados semiestruturados, estruturados ou nao estruturados em um unico lugar em quanto oferecia suporte a uma grande quantidade de trabalhos de data science, machine learning e analise.

Também oferencendo suporte a end-to-end streaming, para relatorios em tempo real.

### A Ascensão da IA generativa.

Para acompanhar as IA's generativas, que avançam e se desenvolvem em velocidades alarmantes Databricks trouxe as duas technologias, Data Lakehouse e Generative IA, para formar a Data Intelligence Platform(Para democratizar data e IA por toda sua organização).

<p align="center">
  <img src="images/databricksDIP.png" width="100">
</p>

---

## What is the Databricks Data Intelligence Platform?

O Objetivo de Databricks sempre foi democratizar a sua tecnologia e compartilhala com outras empresas.

Databricks é pioneira em IA generativa com a aquisição da Mosaic ml em 2023.

Os fundadores de Databricks são os criadores de muitos dos projetos open source mais famosos do mundo usadas em data e IA, como Delta Lake, ML Flow e Apache Spark.

Data e IA são requerimentos para qualquer empresa de sucesso, porém por que é tao dificil ter sucesso nessas areas?

A resposta é que para ter sucesso nessas areas voce precisa comprar varias tecnologias e unificar elas de uma maneira coerente para criar um ambiente ideal para desenvolvimento. Então o que começou com um simples problema de armazenamento, envoluiu para um grande ecossitema de data.

Três problemas principais atrasam empresas:

### 1° Data, IA e Governancia são isoladas.

Um pouco de dados isolados em cada canto do ecossistema dificulta MUITO a governancia,  fazer politicas de segurança e controlar custos de todas essas diferentes plataformas é muito complicado para empresas, e se você juntar IA Generativa, isso so agrega ainda mais ao probleme ao proprio problema.

### 2° IA causa desafios para Privacidade & Controle de dados

A introdução de tanta IA causa problemas em privacidade e controle.

### 3° Altamente dependente em profissionais de alto nivel.

Para fazer tudo isso acontecer, existem muito poucos individuos no mercado de trabalho com habilidades para fazer isso acontecer. Então para empresas funcionarem precisam de empregados de alto nível, e se a empresa nao tem isso, dificilmente terão seus dados e IA desenvolvidos.


#### É justamente ai aonde Data Lake entra.

<p align="center">
  <img src="images/dataecosystem.png" width="100">
</p>

Tendo tudo como uma grande ecossistema e se ajudando, a plataforma de tecnologia que usa Data Lake se torna uma recurso essencial para qualquer empresa quer usar IA ou manipular dados.

<p align="center">
  <img src="images/databricksDIP2.png" width="100">
</p>

#### Open Data Lake

É a base da plataforma.
Aqui ficam armazenados todos os dados brutos da empresa, como:

logs,

textos,

áudios,

vídeos,

imagens,

arquivos diversos

Serve como um “grande lago de dados” centralizado.

Logo, você consegue guardar enormes quantidades de dados sem precisar estruturar tudo antes.

#### Delta Lake

É a camada que organiza e otimiza os dados do Data Lake.

Ela adiciona:

performance,

versionamento,

confiabilidade,

controle de transações

Serve para transformar um Data Lake comum em algo mais seguro e eficiente para análise.

Logo, você consegue consultar dados muito mais rápido e evitar corrupção ou inconsistência.

#### Unity Catalog

É o sistema de governança e controle de dados da Databricks.

Ele controla:

permissões,

segurança,

acesso,

catalogação,

rastreamento dos dados

Serve para organizar quem pode acessar cada informação.

Logo, você consegue gerenciar dados da empresa inteira de forma segura e centralizada.

#### Data Intelligence Engine

É o “cérebro” inteligente da plataforma.

Usa IA generativa para entender:

significado dos dados,

contexto,

relacionamentos

Serve para automatizar análises e facilitar perguntas em linguagem natural.

Logo, você consegue interagir com os dados usando IA sem precisar fazer tudo manualmente.

#### Databricks AI

Área focada em Inteligência Artificial e LLMs.

Permite:

criar modelos,

treinar IA,

ajustar LLMs,

fazer deploy de modelos

Serve para desenvolver soluções de IA personalizadas.

Logo, você consegue construir chatbots, sistemas inteligentes e automações com IA.

#### Delta Live Tables

Ferramenta para criação automática de pipelines de dados.

Ela:

automatiza ETL,

valida qualidade dos dados,

monitora erros

Serve para manter dados sempre atualizados e confiáveis.

Logo, você consegue criar pipelines sem precisar controlar tudo manualmente.

#### Workflows

Sistema de automação e orquestração de tarefas.

Serve para:

agendar jobs,

executar pipelines,

automatizar processos,

controlar execuções

Logo, você consegue criar fluxos automáticos de processamento de dados.

#### Databricks SQL

Ferramenta para análise usando SQL.

Permite:

consultas SQL,

dashboards,

BI,

análise de dados,

Text-to-SQL com IA

Serve para analistas e equipes de negócio explorarem dados facilmente.

Logo, você consegue fazer perguntas em SQL ou até em linguagem natural para analisar informações.


#### Porém também existe uma ferramenta nova que pode usar toda os dados e inteligencia de dados para elevalos um nivel maior
<p align="center">
  <img src="images/projectgenie.png" width="100">
</p>

Similar ao copilot, ele o auxilia para conseguir respostas corretas. 
Ele simplifica sua data plataform.
É inteligente.
É privada, então não existe vazamento.

---