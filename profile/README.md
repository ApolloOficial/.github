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
  <a href="#equipes-e-repositórios">Equipes e repositórios</a> ·
  <a href="#integrantes">Integrantes</a>
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

## Integrantes

Perfis públicos das 12 contas listadas como membros da organização no GitHub.

<table align="center">
  <tr>
    <td align="center"><a href="https://github.com/apollooficial2026-arch"><img src="https://github.com/apollooficial2026-arch.png?size=96" width="72" alt="Perfil de apollooficial2026-arch"><br><strong>apollooficial2026-arch</strong><br><sub>@apollooficial2026-arch</sub></a></td>
    <td align="center"><a href="https://github.com/EnzoDangioMota"><img src="https://github.com/EnzoDangioMota.png?size=96" width="72" alt="Perfil de Enzo Mota"><br><strong>Enzo Mota</strong><br><sub>@EnzoDangioMota</sub></a></td>
    <td align="center"><a href="https://github.com/giquirino"><img src="https://github.com/giquirino.png?size=96" width="72" alt="Perfil de Gi Quirino"><br><strong>Gi Quirino</strong><br><sub>@giquirino</sub></a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/GuiMontonii"><img src="https://github.com/GuiMontonii.png?size=96" width="72" alt="Perfil de Guilherme Montoni"><br><strong>Guilherme Montoni</strong><br><sub>@GuiMontonii</sub></a></td>
    <td align="center"><a href="https://github.com/ikarobueno05"><img src="https://github.com/ikarobueno05.png?size=96" width="72" alt="Perfil de GitIki"><br><strong>GitIki</strong><br><sub>@ikarobueno05</sub></a></td>
    <td align="center"><a href="https://github.com/matheusbotana"><img src="https://github.com/matheusbotana.png?size=96" width="72" alt="Perfil de Matheus Botana"><br><strong>Matheus Botana</strong><br><sub>@matheusbotana</sub></a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/Migs345"><img src="https://github.com/Migs345.png?size=96" width="72" alt="Perfil de Migs345"><br><strong>Migs345</strong><br><sub>@Migs345</sub></a></td>
    <td align="center"><a href="https://github.com/Nichiruto0"><img src="https://github.com/Nichiruto0.png?size=96" width="72" alt="Perfil de Nich Kim"><br><strong>Nich Kim</strong><br><sub>@Nichiruto0</sub></a></td>
    <td align="center"><a href="https://github.com/pczr"><img src="https://github.com/pczr.png?size=96" width="72" alt="Perfil de pczr"><br><strong>pczr</strong><br><sub>@pczr</sub></a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/Sabor-Fernandex"><img src="https://github.com/Sabor-Fernandex.png?size=96" width="72" alt="Perfil de Fernandes"><br><strong>Fernandes</strong><br><sub>@Sabor-Fernandex</sub></a></td>
    <td align="center"><a href="https://github.com/senmdz"><img src="https://github.com/senmdz.png?size=96" width="72" alt="Perfil de Pedro Sena"><br><strong>Pedro Sena</strong><br><sub>@senmdz</sub></a></td>
    <td align="center"><a href="https://github.com/yasbenevenuto"><img src="https://github.com/yasbenevenuto.png?size=96" width="72" alt="Perfil de Yasmin Benevenuto"><br><strong>Yasmin Benevenuto</strong><br><sub>@yasbenevenuto</sub></a></td>
  </tr>
</table>

---

<div align="center">

Projeto Interdisciplinar 2026 · Equipe Apollo ☀️

</div>
