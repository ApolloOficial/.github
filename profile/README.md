# ☀️ Apollo

<p align="center">
  <strong>Plataforma integrada para gestão de ativos fotovoltaicos</strong><br>
  Operação, manutenção e análise em um ecossistema conectado.
</p>

<p align="center">
  <img alt="Apollo" src="https://img.shields.io/badge/APOLLO-Energia_Solar-F15A24?style=for-the-badge&labelColor=292929">
</p>

<p align="center">
  <a href="#ecossistema">Ecossistema</a> ·
  <a href="#equipes-e-repositórios">Equipes e repositórios</a>
</p>

<p align="center">
  <img alt="React" src="https://img.shields.io/badge/React-Interface-61DAFB?logo=react&logoColor=black">
  <img alt="Java" src="https://img.shields.io/badge/Java-Serviços-ED8B00?logo=openjdk&logoColor=white">
  <img alt="Python" src="https://img.shields.io/badge/Python-Automações_e_IA-3776AB?logo=python&logoColor=white">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-Dados-4169E1?logo=postgresql&logoColor=white">
  <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-Eventos-47A248?logo=mongodb&logoColor=white">
  <img alt="Databricks" src="https://img.shields.io/badge/Databricks-Analytics-FF3621?logo=databricks&logoColor=white">
</p>

---

## Ecossistema

Uma iniciativa interdisciplinar desenvolvida por equipes do primeiro e do segundo ano, com requisitos distintos e entregas complementares.

```mermaid
flowchart LR
    people["Técnicos e gestores"] --> web["Apollo Web"]
    people --> mobile["Apollo Mobile"]
    web --> api["Apollo API"]
    mobile --> api
    api --> postgres[("PostgreSQL")]
    api --> assistant["Chatbot ApolloAI"]
    postgres --> bi["Apollo BI"]
    events["Eventos mobile - MongoDB"] --> bi
    bi --> indicators["Indicadores na Web"]
    indicators --> web
    legacy["Banco legado"] --> rpa["RPA de migração"]
    rpa --> postgres
    visitors["Visitantes e equipes"] --> crud["apollo-web-crud"]

    classDef platform fill:#292929,stroke:#F15A24,color:#FFFFFF,stroke-width:2px
    classDef data fill:#FFF2E9,stroke:#F15A24,color:#292929,stroke-width:2px
    class people,web,mobile,api,assistant,bi,indicators,visitors,crud,rpa platform
    class postgres,events data
    class legacy platform
```

## Equipes e repositórios

O **primeiro ano** desenvolve a landing page e a área restrita com operações CRUD. O **segundo ano** desenvolve os sistemas integrados de operação, inteligência artificial, dados e serviços de apoio.

| Repositório | Equipe | Responsabilidade e tecnologias |
| --- | --- | --- |
| [Apollo-Web](https://github.com/ApolloOficial/Apollo-Web) | 2º ano | Painel para ativos, filiais, alertas, ordens de serviço, realocações e indicadores. React, TypeScript e Vite. |
| [apollo-web-crud](https://github.com/ApolloOficial/apollo-web-crud) | 1º ano | Landing page e área restrita com operações CRUD. |
| [Apollo-Mobile](https://github.com/ApolloOficial/Apollo-Mobile) | 2º ano | Aplicativo Android para técnicos em campo: consulta de ativos, leitura de códigos e gestão de problemas e ordens de serviço. |
| [Apollo-API-Spring](https://github.com/ApolloOficial/Apollo-API-Spring) | 2º ano | API REST central para autenticação e operações de negócio. Java, Spring Boot e PostgreSQL. |
| [Chatbot-ApolloAI](https://github.com/ApolloOficial/Chatbot-ApolloAI) | 2º ano | Assistente conversacional integrado à plataforma, com agentes, RAG e memória. Flask, LangChain/LangGraph, Qdrant, MongoDB e Redis. |
| [Access-Log-Api](https://github.com/ApolloOficial/Access-Log-Api) | 2º ano | Serviço para registro e consulta de acessos. Spring Boot e MongoDB. |
| [Apollo-BI](https://github.com/ApolloOficial/Apollo-BI) | 2º ano | Pipeline de dados e indicadores para o dashboard. Databricks, PySpark e Delta Lake. |
| [RPA-data-migration](https://github.com/ApolloOficial/RPA-data-migration) | 2º ano | Automação para validar e migrar cadastros do banco legado para o Apollo. Python. |

---

<div align="center">

Projeto Interdisciplinar 2026 · Equipe Apollo ☀️

</div>
