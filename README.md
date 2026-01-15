# AdventureWorks Databricks Lakehouse Project

## Overview
This project implements a full **Bronze → Silver → Gold Lakehouse architecture**
using **Databricks + PySpark** on the AdventureWorks dataset.

## Architecture
- Bronze Layer: Raw ingestion from CSV
- Silver Layer: Cleaned, conformed data
- Gold Layer:
  - Dimension Tables
  - Fact Tables
  - Aggregated Analytics Tables

## Technologies Used
- Databricks
- PySpark
- Delta Lake

## Data Source
Dataset from Kaggle:
https://www.kaggle.com/datasets/ukveteran/adventure-works

## Folder Structure
- AdventureWorks_Notebooks → Databricks notebooks
- AdventureWorks_Data_Files → Raw CSV files
