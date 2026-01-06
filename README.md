# GCPBigqueyPipeline
This project orchestrate working of batch data ingestion into BigQuery, orchestrated through Airflow and analyzed and shows insights on BI tools

## Architecture
Raw Layer: amazon_sales.csv
||
Processing Layer: Sparks do cleanings of data, joins, scheama validations, aggregations
||
Analytical Layer: Data is ingested to Bigquery to analyze and genrate insights

INPUT(raw data): amazon_sales.csv
|
GCS Bucket(storage)
|
SPARK(Data cleansing, Joins, Agregations, Schema validations)
|
BigQuery(Fast SQL Analytics and BI analytics)
