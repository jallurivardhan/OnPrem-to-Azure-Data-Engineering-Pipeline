# On-Prem to Azure Data Engineering Pipeline

An end-to-end Azure data engineering project that migrates an on-premises SQL Server database to the Azure cloud and builds a complete analytics pipeline — from ingestion to reporting — using modern, secure, and scalable services.

## 🎯 Objective
Automate data movement from on-prem SQL Server to Azure, transform it into analytics-ready datasets, and deliver business insights through Power BI dashboards.

## 🧱 Architecture
![Architecture Diagram](azure-architecture-diagram.png)

**Flow (Bronze → Silver → Gold):**
- **Azure Data Factory**: Orchestrates ingestion from on-prem SQL Server to **Azure Data Lake Gen2** (Bronze).
- **Azure Databricks**: Cleans, enriches, and standardizes data (Silver), then builds business aggregates (Gold).
- **Azure Synapse Analytics**: Exposes Gold data via external tables for fast SQL analytics.
- **Power BI**: Connects to Synapse for dashboards and reports.
- **Azure Key Vault + Entra ID**: Secrets, identity, and access governance across the stack.

## ⚙️ What This Project Includes
- **0_project_setup** – resource setup & connectivity
- **1_data_ingestion** – ADF pipelines, linked services, and datasets
- **2_data_transformation** – Databricks notebooks for Bronze/Silver/Gold
- **3_data_loading** – Synapse SQL views/tables over the lake
- **4_data_reporting** – Power BI model and example dashboard

## 📈 Outcomes
- Automated, repeatable migration from on-prem to cloud
- Lakehouse design with **Bronze/Silver/Gold** layers
- Scalable transformations with Databricks
- Queryable datasets via Synapse
- Shareable insights through Power BI

## 🧰 Skills Demonstrated
Azure Data Factory • Azure Data Lake Gen2 • Azure Databricks • Synapse Analytics • Power BI • Key Vault • Entra ID • SQL • Python • Data Modeling • Governance

## 🔐 Security & Governance
- Secrets managed in **Key Vault**
- Role-based access via **Entra ID**
- Least-privilege access on storage and compute
