 # Decisões Arquiteturais

Este documento registra as principais decisões tomadas ao longo do projeto, com seus respectivos motivos.

---

 ## 📌 Criação manual do Data Lake

Decisão:
- Criar o Data Lake inicialmente via Console AWS

Motivo:
- Foco no entendimento conceitual da arquitetura

---

 ## 📌 Separação entre Landing e Bronze

Decisão:
- Manter camada de Landing separada do medalhão

Motivo:
- Preservar dados brutos
- Facilitar reprocessamento
- Simular necessidades sobre os dados de ambientes corporativos

---

 ## 📌 Uso de GitHub Projects

Decisão:
- Utilizar GitHub Projects (Kanban) para organização do trabalho

Motivo:
- Metodologia ágil
- Garantir rastreabilidade entre tarefas, código e documentação
- Ferramenta integrada ao repositório
