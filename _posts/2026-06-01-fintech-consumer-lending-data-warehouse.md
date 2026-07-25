---
layout: single
title: "Fintech Consumer Lending Data Warehouse & dbt Pipeline"
category: analytical-pipeline-engineering
tools:
  - name: "SQL"
    icon: "fas fa-database"
  - name: "dbt"
    icon: "fas fa-layer-group"
  - name: "GCP BigQuery"
    icon: "fas fa-cloud"
links:
  - title: "GitHub Repository"
    url: "https://github.com/0ladayo/data-modeling-case-studies/tree/main/fintech-lending"
---

Designed a 3NF relational database (OLTP) and translated operational data into a Kimball Star Schema on BigQuery using dbt, decoupling executive reporting from production databases.

**Key Highlights:**
- **Dimensional Architecture**: Implemented SCD Type 2 history tracking for user demography, accumulating snapshot facts for application lifecycles, and transactional ledger facts for repayments.
- **Data Governance & Quality**: Defined dbt schema testing contracts (`unique`, `not_null`, `relationships`, `accepted_values`) across staging and marts layers to enforce referential integrity.
- **Executive KPI Reporting**: Built downstream analytics marts (`rpt_funnel_conversion`, `rpt_user_repayment_risk`) calculating funnel processing velocity and identifying high-risk borrowers.
