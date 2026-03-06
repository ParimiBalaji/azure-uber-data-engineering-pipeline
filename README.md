<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/492cfd68-e6d6-4d7f-8d06-44d39de7f530" />

# azure-uber-data-engineering-pipeline
# Azure Data Engineering Pipeline – Uber Data Analysis

## Project Overview

This project demonstrates the development of a cloud-based data engineering pipeline using Microsoft Azure services. The pipeline ingests multiple Uber ride-related datasets from an HTTP source (GitHub repository) and loads them into Azure Data Lake Storage using Azure Data Factory.

The project uses a metadata-driven ingestion approach where a configuration file (`files_array.json`) dynamically controls which datasets are processed. Azure Data Factory’s Lookup and ForEach activities iterate through the datasets and execute the ingestion pipeline.

## Architecture

The pipeline follows a modern data engineering architecture:

HTTP Source (GitHub)
↓
Azure Data Factory (ETL Pipeline)
↓
Azure Data Lake Storage (Raw Data Storage)

## Technologies Used

* Python
* SQL
* Microsoft Azure Data Factory
* Azure Data Lake Storage
* GitHub
* JSON

## Pipeline Workflow

1. A JSON configuration file contains the list of datasets to be processed.
2. Azure Data Factory Lookup activity reads the configuration file.
3. ForEach activity iterates through each dataset dynamically.
4. Copy Data activity ingests the datasets from GitHub into Azure Data Lake Storage.
5. The pipeline enables scalable and automated data ingestion.

## Key Learning Outcomes

* Building ETL pipelines using Azure Data Factory
* Implementing metadata-driven ingestion pipelines
* Managing cloud-based data storage using Azure Data Lake
* Working with JSON datasets and HTTP sources
* Understanding scalable data pipeline architecture

## Future Improvements

* Data transformation using Azure Databricks
* Data modeling using star schema
* Integration with Power BI for analytics
