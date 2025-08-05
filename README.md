# End-to-End Azure ETL | SQL ➚ ADLS with ADF, Databricks, Synapse & Power BI

## Project Overview

This project demonstrates a complete end-to-end Azure Data Engineering workflow starting from restoring an on-premises SQL Server database to building Power BI dashboards using Medallion architecture in Azure. The project leverages a range of Azure services to build a robust and secure ETL pipeline.

---

## Workflow Diagram

&#x20;

---

## Project Workflow

### 1. Restore & Explore SQL Server Database

- Restored the **AdventureWorks2019** SQL Server database.
- Connected ADF to on-prem SQL using **Self-hosted Integration Runtime**.

### 2. Data Movement to Azure

- Created Azure Data Factory pipelines to dynamically copy multiple tables.
- Raw data stored in **Azure Data Lake Storage Gen2** using the **Bronze, Silver, Gold layers** following Medallion architecture:
  - **Bronze:** Raw data loaded.
  - **Silver:** Cleaned and transformed data.
  - **Gold:** Final curated data exposed as views and external tables.

### 3. Secure Secret Management

- Implemented **Azure Key Vault** for managing credentials securely.
- Used **Key Vault Administrator** role-based access control (RBAC) assigned to user email.

### 4. Data Transformation

- Created **Azure Databricks** workspace and clusters.
- Performed data cleaning and transformation in Databricks.
- Loaded transformed data to the Silver layer.

### 5. Synapse Analytics Integration

- Created **Views** and **External Tables** in **Azure Synapse Analytics**.
- Loaded final data to the Gold layer.

### 6. Data Visualization

- Built **Power BI dashboards** using the external tables created in Synapse.

---

## Resource Provisioning

### Azure Services Created:

- **Resource Group:** Centralized resource management.
- **Azure Data Lake Storage Gen2:** For Medallion architecture storage.
- **Azure Key Vault:** Secure credentials management.
- **Azure Data Factory:** Orchestration of ETL processes.
- **Azure Databricks:** Data transformation and advanced analytics.
- **Azure Synapse Analytics:** Data warehousing and analytics.
- **Power BI:** Data visualization.

### Configurations:

- **Role-based Access Control:**
  - Assigned **Key Vault Administrator** role.
- **Data Factory Pipelines:**
  - Created linked services for source (SQL Server) and sink (ADLS).
  - Used dynamic expressions in pipeline parameterization.
- **Databricks:**
  - Created clusters and configured workspaces for compute activities.

---

## Tech Stack Used

- ✅ **SQL Server 2019** + SSMS
- ✅ **Azure Data Factory (ADF)**
- ✅ **Azure Data Lake Storage Gen2 (ADLS)**
- ✅ **Azure Key Vault**
- ✅ **Azure Databricks**
- ✅ **Azure Synapse Analytics**
- ✅ **Power BI**

---

## Summary

This project showcases how to build an enterprise-grade ETL pipeline on Azure, starting from on-premise data to advanced analytics and visualization:

- Secure
- Scalable
- Maintainable
- Cost-effective

With this architecture, data teams can modernize their data pipelines while leveraging the full power of Microsoft Azure.

---

> I want a readme file format that I can use in my GITHUB repo for the information provided in previous chat. Project is already completed
>
>

