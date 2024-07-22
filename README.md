# Modern Data Engineering with Medallion Architecture

## Project Overview
This project sets up an end-to-end data engineering pipeline using Apache Spark, Azure Databricks, and Data Build Tool (DBT) on the Azure cloud platform. Leveraging the Medallion Architecture, our pipeline encompasses data ingestion, integration, and transformation processes designed to prepare data for advanced analytics.

## Architecture
![System Architecture](System_Architecture.jpeg)

### Components
- **Apache Spark**: Utilized for large-scale data processing.
- **Azure Databricks**: Provides a high-performance analytics platform.
- **DBT (Data Build Tool)**: Used for data modeling and transformations within the data lakehouse.
- **Azure Data Factory**: Manages data pipelines for data integration and transformation.

### Data Layers
- **Bronze**: Raw data ingestion and storage.
- **Silver**: Data cleaning and enrichment.
- **Gold**: Aggregated data optimized for business intelligence.

## Workflow Commands
```bash
dbt run         # Run transformation models
dbt test        # Execute data tests
dbt snapshot    # Manage slowly changing dimensions
dbt docs generate # Generate project documentation
dbt docs serve   # Serve documentation locally
