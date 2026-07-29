# E-Commerce Data Analysis

Projeto de análise de dados desenvolvido utilizando o
Brazilian E-Commerce Public Dataset by Olist.

O objetivo é construir um pipeline completo de dados,
desde a ingestão dos arquivos CSV até a análise e
visualização dos indicadores no Power BI.

## Status do projeto

🚧 Em desenvolvimento

## Tecnologias

- SQL Server
- Pentaho Data Integration
- Python
- Pandas
- Power BI
- Git / GitHub

## Arquitetura

CSV → Pentaho → SQL Server → Python/Pandas → Power BI

## Etapas do projeto

- [x] Análise inicial do dataset
- [x] Modelagem Entidade-Relacionamento (DER)
- [x] Criação do schema STG
- [x] Criação das tabelas de Staging
- [x] Criação das tabelas finais
- [ ] Desenvolvimento do processo ETL
- [ ] Carga dos dados
- [ ] Tratamento e validação
- [ ] Análise exploratória com Python/Pandas
- [ ] Desenvolvimento do dashboard no Power BI
- [ ] Documentação dos insights

## Modelagem de dados

O modelo relacional foi desenvolvido com base nas
relações existentes entre clientes, pedidos, produtos,
vendedores, pagamentos e avaliações.

![DER](docs/der/der_olist.png)

## Banco de dados

O projeto utiliza duas camadas principais:

### STG - Staging

Camada utilizada para receber os dados provenientes
dos arquivos CSV antes do processo de tratamento.

### DBO - Modelo final

Camada que contém as tabelas relacionais tratadas,
com definição de chaves primárias, chaves estrangeiras
e tipos de dados adequados.

## Estrutura do banco

### STG

- stg.customers
- stg.orders
- stg.order_items
- stg.products
- stg.sellers
- stg.payments
- stg.order_reviews
- stg.category_name_translation

### DBO

- dbo.customers
- dbo.orders
- dbo.order_items
- dbo.products
- dbo.sellers
- dbo.payments
- dbo.order_reviews
- dbo.category_name_translation

## Fonte dos dados

Brazilian E-Commerce Public Dataset by Olist
