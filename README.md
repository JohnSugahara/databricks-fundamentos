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
  <img src="images/datawarehouse.png" width="500">
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
  <img src="images/datalake.png" width="500">
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
  <img src="images/datalakehouse.png" width="500">
</p>

Times de empresas ficavam discronizados, usando tecnologias separadas Data Warehouses e Data Lakes causavam problemas de velocidade de entrega.

Para resolver esse problema Databricks matou a necessidade de algo unificado e simples criando o Data Lakehouse.

Combinando os beneficios de um data lake e o poder de analise e controle de um Data Warehouse. Isso criou uma fonta confiavel de dados, combinando acesso direto a IA e BI trabalharem juntos, com uma governancia de segurança unificada.

<p align="center">
  <img src="images/keydatalakehouse.png" width="500">
</p>

Agora empresas podiam guardar, refinar, analisar e acessar dados semiestruturados, estruturados ou nao estruturados em um unico lugar em quanto oferecia suporte a uma grande quantidade de trabalhos de data science, machine learning e analise.

Também oferencendo suporte a end-to-end streaming, para relatorios em tempo real.

### A Ascensão da IA generativa.

Para acompanhar as IA's generativas, que avançam e se desenvolvem em velocidades alarmantes Databricks trouxe as duas technologias, Data Lakehouse e Generative IA, para formar a Data Intelligence Platform(Para democratizar data e IA por toda sua organização).

<p align="center">
  <img src="images/databricksDIP.png" width="500">
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
  <img src="images/dataecosystem.png" width="500">
</p>

Tendo tudo como uma grande ecossistema e se ajudando, a plataforma de tecnologia que usa Data Lake se torna uma recurso essencial para qualquer empresa quer usar IA ou manipular dados.

<p align="center">
  <img src="images/databricksDIP2.png" width="500">
</p>




#### Porém também existe uma ferramenta nova que pode usar toda os dados e inteligencia de dados para elevalos um nivel maior
<p align="center">
  <img src="images/projectgenie.png" width="500">
</p>

Similar ao copilot, ele o auxilia para conseguir respostas corretas. 
Ele simplifica sua data plataform.
É inteligente.
É privada, então não existe vazamento.

---

## Databricks DI Platform Architecture And Security Fundamentals

Neste tópico teremos o objetivo de desenvolver o conhecimento da arquitetura da plataforma.

Antes do resumo de cada parte importante da plataforma vamos falar sobre Delta Lake:

<p align="center">
  <img src="images/deltalake.png" width="500">
</p>

O Delta Lake é uma camada de armazenamento inteligente da Databricks criada para melhorar os Data Lakes tradicionais.
Ele funciona em cima do armazenamento de dados bruto e adiciona recursos avançados de confiabilidade, desempenho e controle.

Em um Data Lake comum, os dados podem ficar desorganizados, duplicados ou inconsistentes com o tempo. O Delta Lake resolve esse problema utilizando:

transações ACID
versionamento de dados
otimização automática
controle de alterações
processamento em batch e streaming ao mesmo tempo

Uma das principais vantagens é o versionamento dos dados.
Isso permite recuperar versões antigas de tabelas, desfazer erros e acompanhar mudanças feitas ao longo do tempo.

Ele também melhora muito a performance das consultas, organizando automaticamente os arquivos e otimizando a forma como os dados são armazenados e lidos.

Além disso, o Delta Lake garante maior confiabilidade em pipelines de dados, evitando corrupção e inconsistências durante escritas simultâneas.

Na prática, ele serve como a base moderna para engenharia de dados, analytics e IA dentro da Databricks.

Logo, você consegue trabalhar com grandes volumes de dados de forma rápida, segura, organizada e escalável.

<p align="center">
  <img src="images/datalakedeltalake.png" width="500">
</p>

#### Apache Spark

O Apache Spark é um motor de processamento de dados distribuído muito usado em Big Data.

Ele permite:

processar enormes volumes de dados,

fazer análises rápidas,

executar machine learning,

trabalhar com streaming

Quando o slide fala que o Delta Lake é “compatible with Apache Spark”, significa que ele funciona integrado ao Spark, aproveitando toda a velocidade e escalabilidade da ferramenta.

Logo, você consegue processar dados massivos com alta performance.

#### Delta Tables

Delta Tables são tabelas especiais criadas usando o formato Delta Lake.

Diferente de arquivos comuns, elas possuem:

versionamento,

histórico de alterações,

controle de transações,

otimização automática

Essas tabelas tornam os dados muito mais confiáveis e organizados.

Por exemplo:

várias pessoas podem escrever dados ao mesmo tempo
consultas ficam mais rápidas
erros podem ser revertidos

Logo, você consegue trabalhar com dados de forma mais segura e eficiente.

#### Transaction Log

O Transaction Log é um registro interno que guarda todas as mudanças feitas nas Delta Tables.

Ele salva informações como:

inserções,

exclusões,

atualizações,

versões antigas

Funciona como um “histórico completo” das operações.

Isso é importante porque garante:

consistência dos dados,

recuperação de falhas,

versionamento,

auditoria

Logo, você consegue rastrear mudanças e restaurar dados caso algo dê errado.

### Unity Catalog

<p align="center">
  <img src="images/unitycatalog.png" width="500">
</p>

Unity Catalog

O Unity Catalog é a camada de governança e segurança da Databricks.
Ele foi criado para centralizar o controle de dados, permissões e recursos de IA em um único lugar.

A ideia principal é unificar toda a gestão dos dados da empresa, mesmo que estejam espalhados em diferentes plataformas, bancos ou clouds.

O que ele faz?

O Unity Catalog controla:

quem pode acessar os dados,

quais tabelas existem,

onde os dados estão,

histórico de uso,

auditoria,

segurança,

governança de IA e Machine Learning

Ele funciona como um “gerenciador central” dos dados da empresa.

#### Unified View

<p align="center">
  <img src="images/unified view.png" width="500">
</p>

Facilita pesquisa, classificação e organização de dados estruturados ou nao estruturados como tambem modelos ML ou pastas alheias.

Um de seus outros beneficios é o Single Permission model. Permite que todos seus dados e IA assets possam ser acessadas em uma unica interface. 

Também possui uma monitoração e geração de relatorios movidos por IA, que concede alertas proativos, data lineage em tempo real, dashboards de generação automatica.

Possui uma clara end-to-end view(tempo real) para data flow e consumo.

### Data Governance

Elementos Principais de Governancia de Dados

<p align="center">
  <img src="images/datagovernance.png" width="500">
</p>

#### Data Governance

É o conjunto de práticas usadas para organizar, proteger e controlar os dados da empresa.

O objetivo é garantir que os dados sejam:

seguros,

confiáveis,

organizados,

acessíveis corretamente,

#### Data Cataloging

Organiza e documenta os dados.

Funciona como um “catálogo” mostrando:

quais dados existem,

onde estão,

para que servem

Logo, facilita encontrar informações rapidamente.

#### Data Classification

Classifica os dados por tipo e sensibilidade.

Exemplos:

dados públicos,

confidenciais,

financeiros,

pessoais

Logo, ajuda a aplicar segurança adequada para cada dado.

#### Auditing Data Entitlements and Access

Monitora quem acessa os dados e quais permissões possui.

Serve para:

auditoria,

rastreamento,

conformidade

Logo, a empresa consegue identificar acessos indevidos.

#### Data Discovery

Ajuda usuários a encontrar dados úteis dentro da organização.

Facilita:

pesquisas,

análises,

reutilização de datasets

Logo, reduz tempo procurando informações.

#### Data Sharing and Collaboration

Permite compartilhar dados entre equipes e sistemas.

Serve para melhorar:

colaboração,

integração,

produtividade

Logo, diferentes áreas conseguem trabalhar com os mesmos dados.

#### Data Lineage

Mostra a origem e o caminho dos dados.

Exibe:

de onde vieram,

transformações realizadas,

destino final

Logo, facilita entender e rastrear pipelines de dados.

#### Data Security

Protege os dados contra acessos indevidos.

Inclui:

permissões,

autenticação,

criptografia

Logo, mantém informações seguras.

#### Data Quality

Garante que os dados estejam corretos e confiáveis.

Verifica:

erros,

duplicações,

inconsistências

Logo, melhora a qualidade das análises e decisões.



#### Hoje em dia, data e AI governance é dificil.

Porem tem problemas ao implementar ecosistemas com governancia.

Visão fragmentada do data estate(Ritmo de inovação reduzido).

Muitas ferramentas para manejar acesso(Risco de data breach aumentada, custos operacionais).

Monitoração e visibilidade incompleta(Risco reputacional).

Falta de compartilhamento entre plataformas(falta de compartilhamento entre plataformas).

<p align="center">
  <img src="images/datagovoffer.png" width="500">
</p>

### Delta Sharing
<p align="center">
  <img src="images/deltasharing.png" width="500">
</p>

O Delta Sharing é uma tecnologia aberta da Databricks usada para compartilhar dados entre empresas, equipes e plataformas de forma segura.

Ele permite compartilhar dados em tempo real sem precisar copiar ou mover arquivos.

Funciona com diferentes ferramentas e clouds, como:

Databricks,

Power BI,

Pandas,

Spark,

Snowflake

O compartilhamento acontece através de permissões controladas, mantendo segurança e governança dos dados.

Logo, empresas conseguem colaborar e acessar os mesmos dados de forma rápida, segura e sem duplicação.

### Data Marketplace

O Data Marketplace é um ambiente onde empresas e usuários podem compartilhar, vender ou consumir conjuntos de dados de forma organizada.

Funciona como um “mercado de dados”, permitindo acessar dados prontos para análise sem precisar coletar tudo manualmente.

No contexto da Databricks, ele facilita:

descoberta de datasets,

compartilhamento seguro,

integração entre empresas,

colaboração de dados

Os dados podem incluir:

informações financeiras,

marketing,

logística,

analytics,

IA

Com governança e permissões controladas.

Logo, empresas conseguem encontrar e utilizar dados externos rapidamente para análises, BI e inteligência artificial.

### Databricks Clean Room

atabricks Clean Rooms

O Databricks Clean Room é um ambiente seguro criado para compartilhar e analisar dados entre empresas sem expor os dados brutos.

Ele permite que diferentes organizações colaborem usando seus dados de forma privada e controlada.

Por exemplo:

duas empresas podem comparar informações,

gerar análises conjuntas,

treinar IA,

fazer marketing compartilhado

Tudo isso sem que uma empresa veja diretamente os dados sensíveis da outra.

O Clean Room utiliza:

governança,

permissões,

isolamento seguro,

controle de acesso

Além disso, funciona integrado ao Unity Catalog e ao Delta Sharing.

Logo, empresas conseguem colaborar e extrair insights juntos mantendo privacidade, segurança e conformidade com leis como LGPD e GDPR.

### Control Panel
<p align="center">
  <img src="images/controlplane.png" width="500">
</p>

#### Control Plane

O Control Plane é a camada de gerenciamento da plataforma.

Ele controla e coordena toda a infraestrutura e os serviços da Databricks, mas normalmente não armazena os dados principais da empresa.

O que o Control Plane faz?

Ele gerencia:

interface web,

notebooks,

autenticação,

permissões,

clusters,

jobs,

APIs,

monitoramento,

Unity Catalog,

orquestração geral

Pense nele como o “centro de comando” da plataforma.

Exemplo prático

Quando você:

cria um cluster,

executa um notebook,

agenda um workflow,

configura permissões

Tudo isso passa pelo Control Plane.

Características,

Gerencia operações,

Coordena recursos,

Controla segurança,

Não processa diretamente os dados grandes

Logo, ele é responsável pela administração da plataforma.

#### Data Plane

O Data Plane é a camada onde o processamento real dos dados acontece.

É nela que:

os dados são lidos,

transformados,

processados,

analisados,

O que o Data Plane envolve?

Inclui:

máquinas virtuais,

clusters Spark,

armazenamento,

execução de queries,

pipelines,

processamento de IA

Ou seja, é o ambiente computacional real.

Exemplo prático

Quando um Spark Job roda:

lê dados do S3,

processa milhões de linhas,

treina um modelo

Tudo isso acontece no Data Plane.

Relação entre os dois

O Control Plane envia comandos e gerencia.

O Data Plane executa o trabalho pesado.

Analogia simples

Imagine um restaurante:

**Control Plane**

Seria:

gerente,

sistema de pedidos,

organização,

controle da cozinha,

**Data Plane**x

Seria:

cozinheiros,

fogão,

preparo real da comida,

Na Databricks

Normalmente:

o Control Plane fica gerenciado pela Databricks
o Data Plane roda na cloud do cliente (AWS, Azure ou GCP)

Isso aumenta:

segurança,

isolamento,

controle dos dados

Logo, os dados sensíveis permanecem na infraestrutura da própria empresa enquanto a Databricks faz o gerenciamento da plataforma.

### User Identity and access

<p align="center">
  <img src="images/controlplane.png" width="500">
</p>

#### Table ACLs Feature

ACLs (Access Control Lists) são regras de permissão aplicadas nas tabelas.

Elas controlam:

quem pode visualizar dados,

quem pode editar,

quem pode deletar,

quem pode executar consultas

Logo, diferentes usuários possuem acessos diferentes dentro da plataforma.

#### IAM Instance Profiles

IAM (Identity and Access Management) é o sistema de permissões da cloud, muito usado na AWS.

Os Instance Profiles permitem que clusters da Databricks acessem recursos da cloud com segurança sem precisar colocar credenciais manualmente.

Exemplo:

acessar S3,

ler arquivos,

salvar dados

Logo, o acesso acontece de forma segura e automatizada.

#### Securely Stored Access Key

São chaves de acesso armazenadas de forma segura.

Essas credenciais podem ser:

tokens,

senhas,

chaves da cloud,

APIs

A Databricks protege essas informações para evitar vazamentos.

Logo, usuários e aplicações conseguem autenticar serviços sem expor credenciais diretamente.

#### Secrets API

A Secrets API é um sistema da Databricks usado para armazenar e acessar informações sensíveis.

Exemplos:

senhas,

tokens,

chaves de API,

credenciais de banco

Ao invés de escrever senhas diretamente no código, elas ficam guardadas em um local seguro.

Logo, aumenta a segurança e evita exposição de informações críticas.


---
## DATASHEET(RESUMOS):

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

