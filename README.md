# NewsAPI-Snowflake-Airflow-Project
Airflow project for querying news through NewsAPI and ingest into Snowflake using AWS and airflow.

This project aims at querying 'covid' related data from News API and ingesting into snowflake in a structered table.

It consists of the following steps.
1. Fetch data from News API in Json format, flatten it and store the data as a parquet file in AWS S3. The code is in the file news_fetcher_etl.py
2. Create database,schema and parquet file format in Snowflake. Create a stage in AWS S3 bucket. Scripts are in the file snowflake_scripts.txt
3. Load the parquet file from S3 bucket and load into snowflake table through copy command
   
