# FMCG Unified Data Pipeline and Analytics Platform on Databricks
End-to-end Databricks data engineering pipeline for an FMCG use case, integrating Atlikon and its acquired startup Sports Bar into a unified, scalable Medallion architecture on AWS S3. It handles messy CSV OLTP data, applies robust data quality rules, incremental processing, and delivers AI-assisted analytics and BI dashboards.
## Introduction
This project addresses the real-world challenge of integrating data from two merged FMCG companies—Atlikon (sports equipment manufacturer) and Sports Bar (energy bar startup)—into a unified, scalable data infrastructure on Databricks. Leveraging AWS S3, Python, PySpark, and SQL, the solution implements a Medallion architecture with automated ETL pipelines, data quality validation, and AI-assisted analytics. The platform enables consolidated business intelligence and reporting across both organizations.
## Architecture
![Project Architecture](project_architecture.png)
## Technologies Used
1. Programming language
   - pthon
   - sql
   - pyspark
2. Cloud
   - AWS S3
3. Data Platform
   - Databricks
   - Databricks Jobs (orchestration)
   - Medallion Architecture (Bronze, Silver, Gold layers)
4. AI Assistant
   - Databricks Genie
## Dataset used
The project uses a star-schema dataset combining sales data from two companies: Atlikon (well-structured, already in bronze–silver–gold layers) and Sports Bar (raw, messy CSV data requiring heavy cleaning and standardization). It reconciles differing schemas, fixes data quality issues, and aligns granular daily Sports Bar facts with Atlon’s monthly-level facts to create unified, reliable analytics and dashboards across both businesses.

here is the dataset used for this project - https://github.com/pranotipatil1703/FMCG-Unified-Data-Pipeline-and-Analytics-Platform-on-Databricks/tree/main/0_Data/Parent_company

## Data Model
image

## Scripts for the project
1. [setup catalog, utilities, dim_date_table creation](1_codes/1_setup)
2. [Dimension Data Processing -Customer data processing, products data processing, pricing data processing ](1_codes/2_dimension_data_processing)
3. [Fact Data processing](1_codes/3_fact_data_processing)
