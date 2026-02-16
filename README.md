> # AWS Pipeline Ecosystem

Projeto de Data Lake e pipeline de dados utilizando serviços nativos da AWS, com foco em arquitetura, governança, organização por camadas (Medallion Architecture) e boas práticas de engenharia de dados.

O projeto foi construído de forma incremental, priorizando entendimento conceitual, decisões arquiteturais claras e documentação desde o início.

---

> ## 🎯 Objetivo do Projeto

Construir um ecossistema de dados em AWS capaz de:
- Armazenar dados históricos de forma organizada
- Preparar o ambiente para ingestão novas fontes
- Catalogar e disponibilizar dados para consumo analítico
- Simular um projeto real com metodologia ágil e rastreabilidade

---

> ## 🧱 Arquitetura (Visão Geral)

- Armazenamento: Amazon S3
- Catálogo de dados: AWS Glue Data Catalog
- Consulta analítica: Amazon Athena
- Orquestração: Apache Airflow
- Organização: Medallion Architecture (Landing, Bronze, Silver, Gold)

Detalhes completos estão disponíveis na pasta `docs/`.

---

> ## 📁 Estrutura do Repositório

```text
aws-pipeline-ecosystem/
├── README.md
├── docs/
│ ├── architecture.md
│ ├── data-lake-zones.md
│ └── decisions.md
```

---

> ## 📌 Status do Projeto

Projeto em desenvolvimento, organizado via GitHub Projects (Kanban), com foco em documentação, arquitetura e evolução incremental.
