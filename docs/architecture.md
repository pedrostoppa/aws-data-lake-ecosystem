 # Arquitetura do Projeto

Este projeto utiliza uma arquitetura de Data Lake baseada em serviços nativos da AWS, priorizando simplicidade, baixo acoplamento e escalabilidade.

A arquitetura foi pensada para permitir ingestão de dados de diferentes fontes, organização por camadas e consumo analítico eficiente.

---

 ## 🧩 Visão Geral da Arquitetura

Fluxo lógico do dado:

Landing (S3)
→ Bronze (S3)
→ Silver (S3)
→ Gold (S3)
→ Consulta via Athena / Consumo BI

---

 ## 🗂️ Componentes Principais

### Amazon S3
Responsável pelo armazenamento de dados em todas as camadas do Data Lake.

### AWS Glue Data Catalog
Responsável por catalogar os dados armazenados no S3, permitindo descoberta e consulta via Athena.

### Amazon Athena
Utilizado para consultas SQL diretamente sobre os dados armazenados no S3.

### Apache Airflow
Responsável pela orquestração dos pipelines de dados (ingestão e processamento).

---

 ## 🧠 Princípios Arquiteturais

- Separação clara de responsabilidades por camada
- Dados imutáveis nas camadas iniciais
- Facilidade de reprocessamento
- Baixo custo operacional
- Documentação como parte do projeto
