# Azure Data Pipeline for Sales Order Processing

## Overview
This project aims to build a robust data pipeline using Azure services to process sales order data from multiple sources. The pipeline automates the ingestion, validation, and storage of order data, ensuring data integrity and providing a foundation for analytics.

## Azure Services Used
- Azure Data Lake Storage Gen2 (ADLS Gen2): For storing raw and processed data
- Azure Data Factory (ADF): For data ingestion and orchestration
- Azure Databricks: For data transformation and validation
- Azure SQL Database: For storing valid order statuses and processed data
- Azure Key Vault: For secure storage of secrets and access keys

## Data Pipeline Architecture
[Insert your architecture diagram here]

## Key Features
- Automated file ingestion from ADLS Gen2 landing folder
- Dynamic handling of input files
- Data validation checks:
  1. No duplicate order_id in orders.csv
  2. Check for valid order_status
- Secure storage of sensitive information using Azure Key Vault
- Scalable data processing using Azure Databricks
- Integration with multiple data sources (ADLS Gen2, Amazon S3, Azure SQL DB)

## Implementation Steps
1. **Resource Creation**: Set up necessary Azure resources (Storage Account, Databricks, Data Factory, SQL Database, Key Vault)
2. **Data Ingestion**: Configure Azure Data Factory to monitor and ingest files from the landing folder
3. **Data Validation**: Implement validation logic in Databricks notebooks
4. **Data Processing**: Transform and process valid data
5. **Data Storage**: Store processed data in appropriate locations (staging or discarded folders)

## Future Enhancements
- Implement real-time data processing capabilities
- Extend the pipeline to handle additional data sources
- Develop advanced analytics and reporting features

## Getting Started
[Add instructions on how to set up and run the project]

## Prerequisites
- Azure subscription
- Access to required Azure services
- Necessary permissions and access keys

[Add any additional sections relevant to your specific implementation]
