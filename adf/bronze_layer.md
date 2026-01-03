## Bronze Layer – Azure Data Factory

The Bronze layer is implemented using Azure Data Factory.

### Pipeline Description
- Source: Raw healthcare CSV file
- Sink: Azure Data Lake Storage Gen2 (Bronze container)
- Activity: Copy Data
- Purpose: Land raw data without transformations

Bronze ingestion is handled by ADF to decouple data ingestion from transformation logic.
Databricks is used only from the Silver layer onwards.
