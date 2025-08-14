---
layout: post
title: "Strava Data Pipeline Project"
category: data-engineering
tools:
  - name: "Python"
    icon: "fab fa-python"
  - name: "GCP"
    icon: "fas fa-cloud"
  - name: "Terraform"
    icon: "fas fa-cogs"
  - name: "dbt"
    icon: "fas fa-cogs"
links:
  - title: "Repository"
    url: "https://github.com/0ladayo/strava-data-pipeline"
  - title: "Dashboard"
    url: "https://lookerstudio.google.com/reporting/c95fa90e-cf5d-4b45-a62d-15fa05ed5dab"
  - title: "Observability"
    url: "https://oladayosiyanbola.grafana.net/public-dashboards/f39bb0d5c6b142f2a0c4c3e36c2f7149"
---

This project is a event-driven ELT data pipeline that extracts data from the Strava API, loads it into Google BigQuery, and then transforms it using dbt. The entire infrastructure is deployed on Google Cloud Platform (GCP) and managed with Terraform.