# ApolloOficial

<p align="center"><strong>Plataforma integrada para gestão de ativos fotovoltaicos</strong></p>

A Apollo reúne aplicações para equipes de operação e manutenção de sistemas solares, serviços de apoio e recursos de análise de dados. Os repositórios dividem responsabilidades e se conectam principalmente pela API central.

## Como os repositórios se conectam

```text
Equipes → Apollo Web / Apollo Mobile → Apollo API → PostgreSQL
                                             ├→ ApolloAI (assistente de IA)
                                             ├→ integrações operacionais
                                             └→ tracking em MongoDB

Access Log API → registros de acesso em MongoDB
PostgreSQL / MongoDB → Apollo BI → indicadores e análises
Banco legado → RPA de migração → banco Apollo
```

## Repositórios

| Repositório | Responsabilidade |
| --- | --- |
| [Apollo-Web](https://github.com/ApolloOficial/Apollo-Web) | Painel web para acompanhar ativos, filiais, alertas, ordens de serviço, realocações e funcionários. React, TypeScript e Vite. |
| [Apollo-Mobile](https://github.com/ApolloOficial/Apollo-Mobile) | Aplicativo Android usado por técnicos para consultar placas, ler códigos e trabalhar com problemas e ordens de serviço. Java, Retrofit, CameraX, ML Kit e WorkManager. |
| [Apollo-API-Spring](https://github.com/ApolloOficial/Apollo-API-Spring) | API REST central: autenticação e operações de negócio consumidas pelo Web e Mobile. Java, Spring Boot e PostgreSQL; integra o assistente ApolloAI e serviços externos. |
| [Chatbot-ApolloAI](https://github.com/ApolloOficial/Chatbot-ApolloAI) | Serviço de IA conversacional integrado à API. Flask, LangChain/LangGraph, RAG com Qdrant, memória MongoDB e Redis para ranking/fila. |
| [Access-Log-Api](https://github.com/ApolloOficial/Access-Log-Api) | Serviço REST dedicado ao registro e consulta dos acessos à plataforma, com Spring Boot e MongoDB. |
| [Apollo-BI](https://github.com/ApolloOficial/Apollo-BI) | Camada analítica em Databricks, PySpark e Delta Lake, que combina dados operacionais para produzir indicadores. |
| [RPA-data-migration](https://github.com/ApolloOficial/RPA-data-migration) | Automação Python para validar e migrar cadastros do PostgreSQL legado para o banco Apollo. |

## Fluxo em resumo

- **Uso diário:** Web e Mobile consomem a Apollo API; ela aplica as regras de negócio e acessa os dados operacionais.
- **Assistente:** a API encaminha conversas ao serviço ApolloAI, que busca contexto e mantém memória conversacional.
- **Apoio e análise:** o Access Log API registra acessos; o Apollo BI consolida dados para análise; o RPA apoia a migração inicial de cadastros.

Acesse a [organização ApolloOficial no GitHub](https://github.com/ApolloOficial) para ver os repositórios e suas documentações.
