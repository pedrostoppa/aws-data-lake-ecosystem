 # Camadas do Data Lake

Este projeto utiliza o padrão de Medallion Architecture, separando os dados em camadas com responsabilidades bem definidas.

---

 ## 🟤 Landing (Zona de Ingestão)

- Dados brutos, conforme recebidos da fonte
- Nenhuma transformação aplicada
- Formatos variados (CSV, JSON, etc.)
- Utilizada como base para reprocessamento e auditoria

---

 ## 🥉 Bronze

- Dados estruturados tecnicamente
- Conversão para formato colunar (Parquet)
- Inclusão de colunas técnicas (ex: data de ingestão)
- Ainda sem regras de negócio

---

 ## 🥈 Silver

- Dados limpos e padronizados
- Aplicação de regras de negócio
- Deduplicação e tratamento de inconsistências
- Base para análises confiáveis

---

 ## 🥇 Gold

- Dados prontos para consumo
- Modelagem analítica (Star Schema)
- Foco em performance e usabilidade
- Camada utilizada por BI e Analytics
