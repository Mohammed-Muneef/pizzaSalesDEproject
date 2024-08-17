

# Pizza Sales Analysis - End-to-End Azure Data Engineering Project

## Project Overview

This project aims to analyze pizza sales data using a robust and scalable data engineering pipeline built on Azure. The pipeline extracts, transforms, and loads (ETL) data from a SQL Server database, processes it using Azure Databricks, and then visualizes the results in Power BI. The insights generated help in understanding sales trends, customer preferences, and other key business metrics.

## Architecture

The project architecture consists of the following components:

1. **SQL Server:**
   - Source of the raw transactional data, including pizza orders, customer information, product details, etc.

2. **Azure Data Factory (ADF):**
   - Orchestrates the data flow from SQL Server to Azure Storage.
   - Ensures automated and scheduled data extraction.

3. **Azure Storage:**
   - Serves as a staging area where the raw data is stored in a big data-friendly format (e.g., CSV, Parquet).

4. **Azure Databricks:**
   - Handles data processing using PySpark for data cleaning, transformation, and feature engineering.
   - Performs data aggregation using Spark SQL to prepare the data for reporting.

5. **Aggregates:**
   - Contains summarized data that has been processed and is ready for analysis.

6. **Power BI:**
   - Connects to the aggregated data to create interactive dashboards and reports.
   - Provides insights into sales trends, customer behavior, product performance, and other key metrics.

## Data Flow

1. **Data Extraction:**
   - Data is extracted from SQL Server using Azure Data Factory.
   - The extracted data is then loaded into Azure Storage.

2. **Data Processing:**
   - Azure Databricks processes the data using PySpark to perform necessary transformations.
   - The transformed data is aggregated using Spark SQL.

3. **Data Visualization:**
   - Aggregated data is loaded into Power BI for visualization.
   - Interactive dashboards are created to analyze pizza sales trends, customer preferences, and other insights.

## Getting Started

### Prerequisites

- **Azure Subscription:** An active Azure subscription is required to set up the resources.
- **SQL Server Database:** Ensure that you have access to a SQL Server database with the pizza sales data.
- **Power BI:** Install Power BI Desktop for creating reports and dashboards (or use Power BI Service for online reports).

### Setup Instructions

1. **Azure Data Factory Setup:**
   - Create a new Azure Data Factory instance.
   - Set up a pipeline to extract data from SQL Server and load it into Azure Storage.

2. **Azure Storage Setup:**
   - Create a storage account in Azure.
   - Ensure the extracted data is stored in a structured format (e.g., CSV or Parquet).

3. **Azure Databricks Setup:**
   - Create an Azure Databricks workspace.
   - Develop notebooks using PySpark for data processing and aggregation.
   - Save the processed data back to Azure Storage or another appropriate location.

4. **Power BI Setup:**
   - Connect Power BI to the processed data.
   - Design and publish dashboards and reports based on business requirements.

