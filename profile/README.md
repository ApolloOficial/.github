# ☀️ ApolloOficial

<p align="center">
  <strong>Plataforma integrada para gestão de ativos fotovoltaicos</strong>
</p>

<p align="center">
  <img alt="React" src="https://img.shields.io/badge/React-Interface-61DAFB?logo=react&logoColor=black">
  <img alt="Java" src="https://img.shields.io/badge/Java-Serviços-ED8B00?logo=openjdk&logoColor=white">
  <img alt="Python" src="https://img.shields.io/badge/Python-Automações_e_IA-3776AB?logo=python&logoColor=white">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-Dados-4169E1?logo=postgresql&logoColor=white">
  <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-Eventos-47A248?logo=mongodb&logoColor=white">
  <img alt="Databricks" src="https://img.shields.io/badge/Databricks-Analytics-FF3621?logo=databricks&logoColor=white">
</p>

A Apollo reúne aplicações para apoiar equipes que operam e fazem a manutenção de sistemas solares. Cada repositório cuida de uma parte da plataforma, desde o uso diário até integrações, análise de dados e migração.

---

## Como funciona

- **Operação:** Web e Mobile consomem a Apollo API, que centraliza as regras de negócio e os dados operacionais.
- **Assistente:** o Chatbot ApolloAI oferece orientação conversacional e integra-se à API.
- **Análise:** o Apollo BI combina dados operacionais do PostgreSQL com eventos de uso do MongoDB e alimenta os indicadores exibidos na Web.
- **Serviços de apoio:** o Access Log API registra acessos, e o RPA auxilia na migração de dados legados.

```text
Técnicos e gestores → Apollo Web / Apollo Mobile → Apollo API → PostgreSQL
                                                       └→ Chatbot ApolloAI
PostgreSQL + eventos mobile no MongoDB → Apollo BI → indicadores na Web
Banco legado → RPA de migração → banco Apollo
```

## Repositórios

| Repositório | Responsabilidade |
| --- | --- |
| [Apollo-Web](https://github.com/ApolloOficial/Apollo-Web) | Painel web para ativos, filiais, alertas, ordens de serviço, realocações e indicadores. React, TypeScript e Vite. |
| [Apollo-Mobile](https://github.com/ApolloOficial/Apollo-Mobile) | Aplicativo Android de apoio aos técnicos em campo, com consulta de ativos, leitura de códigos e gestão de problemas e ordens de serviço. |
| [Apollo-API-Spring](https://github.com/ApolloOficial/Apollo-API-Spring) | API REST central para autenticação e operações de negócio. Java, Spring Boot e PostgreSQL. |
| [Chatbot-ApolloAI](https://github.com/ApolloOficial/Chatbot-ApolloAI) | Assistente conversacional integrado à plataforma, com agentes, RAG e memória de conversa. Flask, LangChain/LangGraph, Qdrant, MongoDB e Redis. |
| [Access-Log-Api](https://github.com/ApolloOficial/Access-Log-Api) | Serviço para registro e consulta de acessos, com Spring Boot e MongoDB. |
| [Apollo-BI](https://github.com/ApolloOficial/Apollo-BI) | Pipeline de dados e indicadores para o dashboard, usando Databricks, PySpark e Delta Lake. |
| [RPA-data-migration](https://github.com/ApolloOficial/RPA-data-migration) | Automação Python para validar e migrar cadastros do banco legado para o Apollo. |

---

<div align="center">

Projeto Interdisciplinar 2026 · Equipe Apollo ☀️

</div>
