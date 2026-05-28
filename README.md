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
  <img src="datawarehouse.png" width="100">
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
  <img src="datalake.png" width="100">
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
  <img src="datalakehouse.png" width="100">
</p>

Times de empresas ficavam discronizados, usando tecnologias separadas Data Warehouses e Data Lakes causavam problemas de velocidade de entrega.

Para resolver esse problema Databricks matou a necessidade de algo unificado e simples criando o Data Lakehouse.

Combinando os beneficios de um data lake e o poder de analise e controle de um Data Warehouse. Isso criou uma fonta confiavel de dados, combinando acesso direto a IA e BI trabalharem juntos, com uma governancia de segurança unificada.

<p align="center">
  <img src="keydatalakehouse.png" width="100">
</p>

Agora empresas podiam guardar, refinar, analisar e acessar dados semiestruturados, estruturados ou nao estruturados em um unico lugar em quanto oferecia suporte a uma grande quantidade de trabalhos de data science, machine learning e analise.

Também oferencendo suporte a end-to-end streaming, para relatorios em tempo real.

### A Ascensão da IA generativa.

Para acompanhar as IA's generativas, que avançam e se desenvolvem em velocidades alarmantes Databricks trouxe as duas technologias, Data Lakehouse e Generative IA, para formar a Data Intelligence Platform(Para democratizar data e IA por toda sua organização).

<p align="center">
  <img src="databricksDIP.png" width="100">
</p>

---

## What is the Databricks Data Intelligence Platform?

