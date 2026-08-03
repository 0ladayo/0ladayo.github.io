---
layout: single
title: "End-to-End Data Modeling: Oil & Gas Case Study"
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
    url: "https://github.com/0ladayo/data-modeling-case-studies/tree/main/end-to-end%20modelling%3B%20oil%20and%20gas%20case%20study"
  - title: "Part 1: Relational Modeling (3NF)"
    url: "https://medium.com/data-engineer-things/from-flat-files-to-relational-models-architecting-oil-gas-production-data-8c9c1e684408"
  - title: "Part 2: Dimensional Modeling (Star Schema)"
    url: "https://medium.com/@Oladayo/from-relational-models-to-dimension-models-architecting-oil-gas-production-data-26a9c780e686/"
---

Designed a normalized 3NF operational database schema and transformed it into a Kimball dimensional star schema on BigQuery using dbt.

**Key Highlights:**
- **3NF Relational Schema Design**: Architected a normalized PostgreSQL schema (fields, reservoirs, wells, and daily volume metrics) to enforce data constraints and track operational hierarchy.
- **SCD Type 2 History Tracking**: Implemented dbt snapshots to track status updates over time (drilling → producing → shut-in) without overwriting historical data.
- **Point-in-Time Star Schema**: Built `dim_wells` and `fct_production` using point-in-time joins so daily production metrics accurately match the well's status on that specific date.