# Azure Data Engineering End-to-End Project
## Project Overview
This is an end to end Data Engineering project. The project involves fetching the data from source using API, Ingestting the data to Azure data Lake Gen2(Bronze layer) and processing it using pyspark for further transformation and analysis. Project demonstrates the architecture and implementation of a data pipeline using Azure services.

## Architecture

<img width="552" alt="image" src="https://github.com/user-attachments/assets/e563f408-4ff8-432f-bbf0-aac3b94fa185" />

## Key Component
### 1. Azure Data Factory
Azure Data Factory serves as the orchestrator for the data pipeline, managing the data movement and transformation processes. It ensures seamless integration between different data sources and destinations.
### 2. Live Mode
The pipeline supports real-time data processing capabilities, enabling timely ingestion and processing of data as it becomes available.
### 3. ETL (Extract, Transform, Load)
The ETL process is a critical component of the pipeline, responsible for:
Extracting data from various sources using APIs.
Transforming the data into a suitable format for analysis.
Loading the transformed data into Azure Data Lake Gen2.
### 4. Azure Data Lake Gen2
Azure Data Lake Gen2 is utilized for storing large volumes of raw and processed data. The data is organized into different layers:
Bronze Layer: Raw data ingested from various sources.
Silver Layer: Cleaned and transformed data.
Gold Layer: Aggregated and enriched data ready for analysis.
### 5. PySpark
PySpark is employed for big data processing, leveraging the power of Apache Spark with Python. It facilitates efficient data transformation and analysis.
### 6. API Integration
APIs are used to fetch data from external sources, ensuring the pipeline can ingest diverse datasets. The integration with APIs allows for dynamic and scalable data ingestion.

## Workflow
### 1. Data Ingestion
The pipeline fetches raw data from external sources using APIs and copy it to Azure data lake Gen2(Bronze layer), enabling dynamic and scalable data ingestion. It ensure seamless integration between different data sources and destinations. 

API Integration: APIs are used to fetch data from various external sources. This allows the pipeline to ingest diverse datasets in real-time.
Bronze Layer: Raw data ingested from various sources is stored in Azure Data Lake Gen2's Bronze layer. This layer serves as the initial storage for unprocessed data.

