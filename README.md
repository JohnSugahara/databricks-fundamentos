# Databricks e seus Fundamentos

## Tópicos

### 1° Historia das plataformas de manejamento de dados.

### 2° O que é a Plataforma Databricks Intelligence?

### 3° Arquitetura da Plataforma Databricks DI e Fundamentais de Segurança.

- *a.* Visão geral da arquitetura da plataforma.
- *b.* Data governance.
- *c.* Segurança, Confiabilidade e Performance.
- *d.* The Data Intelligence Engine

### 4° Workloads suportadas na Plataforma Databricks DI

- *a.* Data warehousing
- *b.* Orchestration
- *c.* ETL & analise tempo-real
- *d.* Data science & AI

### 5° Sumário e Proximos passos.

---

## The History of Data Management Platforms

### No fim dos anos 80 (1980), empresas queriam possuir as percepções movidas por dados (*data-driven insights*) para decisões empresariais e inovação.

Para isso, organizações precisavam sair dos dados coletados apenas por simples bases relacionais para sistemas que manejavam e analisavam dados sendo gerados em tempo real e em grandes volumes com alta velocidade.

<p align="center">
  <img src="images/datawarehouse.png" width="500">
</p>

**Data Warehouses** foram criados para coletar e consolidar o fluxo de dados e prover suporte geral para dados de inteligência e análise de empresas.

Dados e Data Warehouses eram estruturados e limpos, com esquemas pré-definidos. Porém, Data Warehouses não foram feitos com dados semiestruturados ou não estruturados em mente — dessa forma, não havia suporte para dados fora do padrão correto.

Isso causou:

- Inflexibilidade em esquemas
- Problemas com pico de volume e velocidade
- Longo tempo de processamento

Com o avanço do mundo digital, isso apenas piorou, pois os dados aumentaram em volume, velocidade e variedade. O que desfavoreceu as Data Warehouses: tomava muito tempo para processar dados e prover resultados, e havia capacidade limitada para lidar com variedade e velocidade de dados.

---

### Em 2000 houve a ascensão de algo chamado **"Big Data"**, ocasionando a criação dos **Data Lakes**.

O Data Lake permitia que dados estruturados, semiestruturados e não estruturados convivessem no mesmo ambiente simultaneamente — coletados em volume e velocidade necessários para dar suporte ao ritmo de geração de dados da época.

<p align="center">
  <img src="images/datalake.png" width="500">
</p>

Diversos dados diferentes poderiam ser guardados lado a lado em um Data Lake. Dados criados de diferentes origens — sejam logs de web ou dados de sensores — poderiam ser transmitidos para o Data Lake com facilidade, velocidade e de maneira barata em armazenamento de objetos cloud de baixo preço.

Apesar dos Data Lakes resolverem o problema de armazenamento, eles criaram novos problemas — não possuíam coisas essenciais que Data Warehouses tinham:

- **Sem suporte para dados transacionais** e sem capacidade de reforçar qualidade de dados — baixa confiança nos dados
- **Velocidade de análise lenta** pela alta quantidade de dados — a oportunidade de decisões com impacto nunca se manifestou
- **Governança de dados desafiadora** para reforço de segurança e privacidade, pela falta de estrutura

---

### Em 2021 ocorreu a ascensão do paradigma da arquitetura **LakeHouse**.

Em 2013, a Databricks foi fundada. Em 2020, introduziu ao mundo a primeira e única Plataforma Lakehouse em Cloud, combinando os melhores aspectos de Data Warehouses e Data Lakes em uma plataforma unificada e aberta para dados e IA.

Em 2021, os fundadores da Databricks e outros indivíduos cunharam o termo **"Arquitetura Lakehouse"** no artigo:

> *"Lakehouse: A nova geração de plataformas abertas que unificam Data Warehousing e Análise Avançada"*

<p align="center">
  <img src="images/datalakehouse.png" width="500">
</p>

Times de empresas ficavam desincronizados — usar tecnologias separadas de Data Warehouses e Data Lakes causava problemas de velocidade de entrega.

Para resolver esse problema, a Databricks identificou a necessidade de algo **unificado e simples**, criando o Data Lakehouse: combinando os benefícios de um Data Lake com o poder de análise e controle de um Data Warehouse. Isso criou uma fonte confiável de dados, combinando acesso direto a IA e BI trabalhando juntos, com governança de segurança unificada.

<p align="center">
  <img src="images/keydatalakehouse.png" width="500">
</p>

Agora, empresas podiam guardar, refinar, analisar e acessar dados semiestruturados, estruturados ou não estruturados em um único lugar, enquanto oferecia suporte a uma grande quantidade de trabalhos de Data Science, Machine Learning e análise. Também oferecendo suporte a end-to-end streaming para relatórios em tempo real.

---

### A Ascensão da IA Generativa

Para acompanhar as IAs generativas — que avançam e se desenvolvem em velocidades alarmantes — a Databricks trouxe as duas tecnologias, **Data Lakehouse** e **IA Generativa**, para formar a **Data Intelligence Platform** (para democratizar dados e IA por toda a organização).

<p align="center">
  <img src="images/databricksDIP.png" width="500">
</p>

---

## What is the Databricks Data Intelligence Platform?

O objetivo da Databricks sempre foi democratizar sua tecnologia e compartilhá-la com outras empresas.

A Databricks é pioneira em IA generativa, com a aquisição da **Mosaic ML em 2023**.

Os fundadores da Databricks são os criadores de muitos dos projetos open source mais famosos do mundo usados em dados e IA, como **Delta Lake**, **MLflow** e **Apache Spark**.

Dados e IA são requisitos para qualquer empresa de sucesso. Mas por que é tão difícil ter sucesso nessas áreas?

A resposta é que para ter sucesso é necessário comprar várias tecnologias e unificá-las de maneira coerente para criar um ambiente ideal de desenvolvimento. Então o que começou com um simples problema de armazenamento evoluiu para um grande ecossistema de dados.

**Três problemas principais atrasam empresas:**

### 1° Data, IA e Governança são isoladas

Um pouco de dados isolados em cada canto do ecossistema dificulta MUITO a governança. Fazer políticas de segurança e controlar custos de todas essas diferentes plataformas é muito complicado, e se você juntar IA Generativa, isso só agrega ainda mais ao problema.

### 2° IA causa desafios para Privacidade & Controle de dados

A introdução de tanta IA causa problemas de privacidade e controle.

### 3° Altamente dependente em profissionais de alto nível

Para fazer tudo isso acontecer, existem muito poucos indivíduos no mercado de trabalho com habilidades para tal. Então, para as empresas funcionarem, precisam de empregados de alto nível — e se não os têm, dificilmente terão seus dados e IA desenvolvidos.

---

#### É justamente aí onde a Databricks Data Intelligence Platform entra.

<p align="center">
  <img src="images/dataecosystem.png" width="500">
</p>

Tendo tudo como um grande ecossistema integrado e colaborativo, a plataforma se torna um recurso essencial para qualquer empresa que queira usar IA ou manipular dados.

<p align="center">
  <img src="images/databricksDIP2.png" width="500">
</p>

#### Também existe uma ferramenta nova que eleva toda a plataforma a um nível maior: o **Project Genie**

<p align="center">
  <img src="images/projectgenie.png" width="500">
</p>

Similar ao Copilot, ele auxilia a conseguir respostas corretas a partir dos dados. É:

- **Simples** — simplifica sua data platform
- **Inteligente** — entende o contexto da organização
- **Privado** — não existe vazamento de informações sensíveis

---

## Databricks DI Platform Architecture and Security Fundamentals

Neste tópico o objetivo é desenvolver o conhecimento da arquitetura da plataforma.

Antes do resumo de cada parte importante, vamos falar sobre **Delta Lake**:

<p align="center">
  <img src="images/deltalake.png" width="500">
</p>

O **Delta Lake** é uma camada de armazenamento inteligente da Databricks criada para melhorar os Data Lakes tradicionais. Ele funciona em cima do armazenamento de dados bruto e adiciona recursos avançados de confiabilidade, desempenho e controle.

Em um Data Lake comum, os dados podem ficar desorganizados, duplicados ou inconsistentes com o tempo. O Delta Lake resolve esse problema utilizando:

- Transações ACID
- Versionamento de dados
- Otimização automática
- Controle de alterações
- Processamento em batch e streaming ao mesmo tempo

Uma das principais vantagens é o **versionamento dos dados** — permite recuperar versões antigas de tabelas, desfazer erros e acompanhar mudanças feitas ao longo do tempo.

Ele também melhora muito a **performance das consultas**, organizando automaticamente os arquivos e otimizando a forma como os dados são armazenados e lidos.

Além disso, o Delta Lake garante maior **confiabilidade em pipelines de dados**, evitando corrupção e inconsistências durante escritas simultâneas.

Na prática, ele serve como a base moderna para engenharia de dados, analytics e IA dentro da Databricks — permitindo trabalhar com grandes volumes de dados de forma rápida, segura, organizada e escalável.

<p align="center">
  <img src="images/datalakedeltalake.png" width="500">
</p>

### Apache Spark

O **Apache Spark** é um motor de processamento de dados distribuído muito usado em Big Data. Ele permite:

- Processar enormes volumes de dados
- Fazer análises rápidas
- Executar machine learning
- Trabalhar com streaming

Quando se diz que o Delta Lake é *"compatible with Apache Spark"*, significa que ele funciona integrado ao Spark, aproveitando toda a velocidade e escalabilidade da ferramenta — permitindo processar dados massivos com alta performance.

### Delta Tables

**Delta Tables** são tabelas especiais criadas usando o formato Delta Lake. Diferente de arquivos comuns, elas possuem:

- Versionamento
- Histórico de alterações
- Controle de transações
- Otimização automática

Essas tabelas tornam os dados muito mais confiáveis e organizados. Por exemplo: várias pessoas podem escrever dados ao mesmo tempo, consultas ficam mais rápidas e erros podem ser revertidos.

### Transaction Log

O **Transaction Log** é um registro interno que guarda todas as mudanças feitas nas Delta Tables. Ele salva informações como:

- Inserções
- Exclusões
- Atualizações
- Versões antigas

Funciona como um "histórico completo" das operações, garantindo consistência dos dados, recuperação de falhas, versionamento e auditoria.

---

### Unity Catalog

<p align="center">
  <img src="images/unitycatalog.png" width="500">
</p>

O **Unity Catalog** é a camada de governança e segurança da Databricks. Foi criado para centralizar o controle de dados, permissões e recursos de IA em um único lugar.

A ideia principal é **unificar toda a gestão dos dados da empresa**, mesmo que estejam espalhados em diferentes plataformas, bancos ou clouds.

**O Unity Catalog controla:**

- Quem pode acessar os dados
- Quais tabelas existem
- Onde os dados estão
- Histórico de uso
- Auditoria
- Segurança
- Governança de IA e Machine Learning

Ele funciona como um "gerenciador central" dos dados da empresa.

#### Unified View

<p align="center">
  <img src="images/unified view.png" width="500">
</p>

Facilita pesquisa, classificação e organização de dados estruturados ou não estruturados, como também modelos ML ou pastas diversas.

Um de seus outros benefícios é o **Single Permission Model** — permite que todos os dados e AI assets possam ser acessados em uma única interface.

Também possui uma **monitoração e geração de relatórios movidos por IA**, que concede alertas proativos, data lineage em tempo real e dashboards de geração automática — com uma clara visão end-to-end (tempo real) do fluxo e consumo de dados.

---

### Data Governance

**Elementos Principais de Governança de Dados**

<p align="center">
  <img src="images/datagovernance.png" width="500">
</p>

**Data Governance** é o conjunto de práticas usadas para organizar, proteger e controlar os dados da empresa, garantindo que sejam seguros, confiáveis, organizados e acessíveis corretamente.

#### Data Cataloging

Organiza e documenta os dados. Funciona como um "catálogo" mostrando quais dados existem, onde estão e para que servem — facilitando encontrar informações rapidamente.

#### Data Classification

Classifica os dados por tipo e sensibilidade — dados públicos, confidenciais, financeiros, pessoais — ajudando a aplicar segurança adequada para cada tipo.

#### Auditing Data Entitlements and Access

Monitora quem acessa os dados e quais permissões possui. Serve para auditoria, rastreamento e conformidade — permitindo identificar acessos indevidos.

#### Data Discovery

Ajuda usuários a encontrar dados úteis dentro da organização, facilitando pesquisas, análises e reutilização de datasets — reduzindo tempo procurando informações.

#### Data Sharing and Collaboration

Permite compartilhar dados entre equipes e sistemas, melhorando colaboração, integração e produtividade — possibilitando que diferentes áreas trabalhem com os mesmos dados.

#### Data Lineage

Mostra a origem e o caminho dos dados: de onde vieram, transformações realizadas e destino final — facilitando entender e rastrear pipelines de dados.

#### Data Security

Protege os dados contra acessos indevidos com permissões, autenticação e criptografia.

#### Data Quality

Garante que os dados estejam corretos e confiáveis, verificando erros, duplicações e inconsistências — melhorando a qualidade das análises e decisões.

---

#### Hoje em dia, data e AI governance é difícil.

Existem problemas ao implementar ecossistemas com governança:

- **Visão fragmentada do data estate** → ritmo de inovação reduzido
- **Muitas ferramentas para manejar acesso** → risco de data breach aumentado e custos operacionais elevados
- **Monitoração e visibilidade incompleta** → risco reputacional
- **Falta de compartilhamento entre plataformas** → silos de dados

<p align="center">
  <img src="images/datagovoffer.png" width="500">
</p>

---

### Delta Sharing

<p align="center">
  <img src="images/deltasharing.png" width="500">
</p>

O **Delta Sharing** é uma tecnologia aberta da Databricks usada para compartilhar dados entre empresas, equipes e plataformas de forma segura. Ele permite compartilhar dados em tempo real **sem precisar copiar ou mover arquivos**.

Funciona com diferentes ferramentas e clouds, como Databricks, Power BI, Pandas, Spark e Snowflake. O compartilhamento acontece através de permissões controladas, mantendo segurança e governança dos dados.

### Data Marketplace

O **Data Marketplace** é um ambiente onde empresas e usuários podem compartilhar, vender ou consumir conjuntos de dados de forma organizada. Funciona como um "mercado de dados", permitindo acessar dados prontos para análise sem precisar coletar tudo manualmente.

No contexto da Databricks, ele facilita:

- Descoberta de datasets
- Compartilhamento seguro
- Integração entre empresas
- Colaboração de dados

Os dados podem incluir informações financeiras, de marketing, logística, analytics e IA — com governança e permissões controladas.

### Databricks Clean Room

O **Databricks Clean Room** é um ambiente seguro criado para compartilhar e analisar dados entre empresas **sem expor os dados brutos**. Permite que diferentes organizações colaborem usando seus dados de forma privada e controlada.

Por exemplo: duas empresas podem comparar informações, gerar análises conjuntas, treinar IA ou fazer marketing compartilhado — tudo isso sem que uma empresa veja diretamente os dados sensíveis da outra.

O Clean Room utiliza governança, permissões, isolamento seguro e controle de acesso. Funciona integrado ao Unity Catalog e ao Delta Sharing, garantindo conformidade com leis como **LGPD** e **GDPR**.

---

### Control Plane

<p align="center">
  <img src="images/controlplane.png" width="500">
</p>

O **Control Plane** é a camada de gerenciamento da plataforma. Ele controla e coordena toda a infraestrutura e os serviços da Databricks, mas normalmente não armazena os dados principais da empresa.

**O que o Control Plane gerencia:**

- Interface web
- Notebooks
- Autenticação e permissões
- Clusters e jobs
- APIs
- Monitoramento
- Unity Catalog
- Orquestração geral

Pense nele como o **"centro de comando"** da plataforma. Quando você cria um cluster, executa um notebook, agenda um workflow ou configura permissões — tudo passa pelo Control Plane.

#### Data Plane

O **Data Plane** é a camada onde o processamento real dos dados acontece. É nela que os dados são lidos, transformados, processados e analisados. Inclui máquinas virtuais, clusters Spark, armazenamento, execução de queries, pipelines e processamento de IA.

Quando um Spark Job roda — lê dados do S3, processa milhões de linhas, treina um modelo — tudo acontece no Data Plane.

**Relação entre os dois:**

- O **Control Plane** envia comandos e gerencia
- O **Data Plane** executa o trabalho pesado

> Analogia: em um restaurante, o Control Plane seria o gerente e o sistema de pedidos; o Data Plane seriam os cozinheiros e o fogão.

Na Databricks, normalmente o Control Plane fica gerenciado pela Databricks, enquanto o Data Plane roda na cloud do cliente (AWS, Azure ou GCP) — aumentando segurança, isolamento e controle dos dados. Os dados sensíveis permanecem na infraestrutura da própria empresa.

---

### User Identity and Access

<p align="center">
  <img src="images/controlplane.png" width="500">
</p>

#### Table ACLs Feature

**ACLs (Access Control Lists)** são regras de permissão aplicadas nas tabelas. Elas controlam quem pode visualizar, editar, deletar ou executar consultas — garantindo que diferentes usuários possuam acessos diferentes dentro da plataforma.

#### IAM Instance Profiles

**IAM (Identity and Access Management)** é o sistema de permissões da cloud, muito usado na AWS. Os Instance Profiles permitem que clusters da Databricks acessem recursos da cloud com segurança — como acessar S3, ler arquivos e salvar dados — sem precisar colocar credenciais manualmente.

#### Securely Stored Access Key

São chaves de acesso armazenadas de forma segura — tokens, senhas, chaves da cloud, APIs. A Databricks protege essas informações para evitar vazamentos, permitindo que usuários e aplicações autentiquem serviços sem expor credenciais diretamente.

#### Secrets API

A **Secrets API** é um sistema da Databricks usado para armazenar e acessar informações sensíveis como senhas, tokens, chaves de API e credenciais de banco. Ao invés de escrever senhas diretamente no código, elas ficam guardadas em um local seguro — aumentando a segurança e evitando exposição de informações críticas.

---

### Databricks Serverless SQL

<p align="center">
  <img src="images/Databricks Serverless SQL.png" width="500">
</p>

O **Databricks Serverless SQL** é um serviço de SQL totalmente gerenciado pela Databricks, onde você não precisa criar, configurar ou manter clusters manualmente.

O termo *"serverless"* significa exatamente isso: sem gerenciar servidores, sem configurar infraestrutura, sem administrar máquinas — a Databricks faz tudo automaticamente em segundo plano.

**Permite executar:**

- Consultas SQL
- Dashboards
- BI e analytics
- Queries em Big Data

de forma rápida e automática. É muito usado por analistas de dados, equipes de BI, dashboards corporativos e relatórios em tempo real.

**Problemas que ele resolve:**

**1. Elimina gerenciamento de clusters**
Antes era necessário criar cluster, configurar máquinas, escolher tamanho e monitorar recursos. Com Serverless, tudo é automático — reduzindo complexidade operacional.

**2. Resolve problemas de escalabilidade**
Se muitos usuários executarem consultas ao mesmo tempo, o Serverless escala automaticamente — aumenta recursos, distribui carga e otimiza performance, evitando lentidão em horários de pico.

**3. Reduz custo**
Clusters tradicionais podem ficar ligados sem uso. O Serverless inicia sob demanda, desliga automaticamente e cobra apenas pelo uso real — reduzindo desperdício de infraestrutura.

**4. Melhora performance SQL**
A Databricks otimiza automaticamente cache, execução, recursos computacionais e paralelismo — consultas ficam mais rápidas sem ajustes manuais.

**5. Facilita BI e Analytics**
Ferramentas como Power BI, Tableau e Looker podem conectar diretamente — analistas conseguem consultar grandes volumes de dados sem depender da equipe de infraestrutura.

**Como funciona internamente:**

Quando alguém executa uma query, a Databricks cria recursos automaticamente, executa a consulta, otimiza performance e libera recursos quando termina — tudo sem o usuário gerenciar servidores.

**Relação com Data Lakehouse:**

O Serverless SQL acessa dados armazenados em Delta Lake, Unity Catalog e Data Lakes — permitindo usar SQL diretamente sobre grandes volumes de dados modernos.

**Diferença para cluster tradicional:**

| | Cluster Tradicional | Serverless SQL |
|---|---|---|
| Gerenciamento | Você cria, configura e monitora | Databricks gerencia tudo |
| Escalabilidade | Manual | Automática |
| Custo | Paga mesmo parado | Paga apenas pelo uso |

---

### O que é Photon?

<p align="center">
  <img src="images/photon.png" width="500">
</p>

O **Photon** é o mecanismo de processamento de alta performance da Databricks, criado para acelerar consultas SQL, processamento Spark, analytics e Data Engineering usando otimizações em baixo nível.

**O que ele resolve:**

- Lentidão em consultas
- Alto consumo de recursos
- Processamento ineficiente de Big Data

Ele melhora velocidade, paralelismo, uso de CPU e performance de queries — tornando workloads muito mais rápidos e baratos.

**Como funciona:**

O Photon substitui partes do processamento tradicional do Spark por um engine otimizado em **C++**, permitindo melhor uso do hardware, execução vetorizada e processamento mais eficiente.

**Onde é usado:**

- Databricks SQL
- ETL e pipelines de dados
- Data Warehousing
- Analytics em larga escala

**Benefícios:**

- Queries mais rápidas
- Menor custo computacional
- Melhor escalabilidade
- Performance otimizada automaticamente

**Relação com Spark:**

O Photon funciona integrado ao Apache Spark — o Spark continua sendo usado e o Photon acelera a execução interna. Usuários conseguem mais performance sem mudar seus códigos SQL ou Spark.