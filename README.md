# AdventureWorks Databricks Lakehouse Project

## Overview
This project demonstrates an end-to-end Retail Analytics Platform built using Databricks, Delta Lake, and PySpark, following the Medallion Architecture (Bronze → Silver → Gold).

The solution processes raw AdventureWorks retail data and transforms it into clean, governed, and analytics-ready datasets, enabling fast analytical queries and BI reporting through a star schema design.

The project closely mirrors real-world enterprise data engineering practices which includes layered data modeling, incremental transformations and job orchestration using Databricks Workflows.
  ### Note:
   - This project conceptually follows an AWS-based architecture using Amazon S3 as the raw data source. However, due to limitations of the Databricks Community Edition          (which does not support direct cloud storage integrations), the actual implementation uses Databricks-managed storage to simulate the S3 ingestion layer.
   - The overall architecture, data modeling, transformations, and optimization techniques remain aligned with real-world, production-grade data engineering practices.


## Architecture
- Bronze Layer: Raw ingestion from CSV
- Silver Layer: Cleaned, conformed data
- Gold Layer:
  - Dimension Tables
  - Fact Tables
  - Aggregated Analytics Tables
 
## Highlights
- Implemented Medallion Architecture using Delta Lake
- Designed Bronze, Silver, and Gold layers
- Combined multiple yearly sales datasets into a unified fact table
- Built Fact and Dimension tables using star schema
- Created analytics-ready Gold tables
- Orchestrated pipelines using Databricks Jobs

## Technologies Used
-Databricks – Distributed data processing & analytics
- Delta Lake – Reliable, ACID-compliant data storage
- Unity Catalog – Centralized governance and schema management
- Apache Spark (PySpark) – Data transformations and cleaning
- SQL – Analytics & aggregations
- AWS – S3 note: it was not used as we are using databricks community edition
- Medallion Architecture – Scalable data design pattern

## Data Source
Dataset from Kaggle:
https://www.kaggle.com/datasets/ukveteran/adventure-works

## Folder Structure
- AdventureWorks_Notebooks → Databricks notebooks
- AdventureWorks_Data_Files → Raw CSV files
