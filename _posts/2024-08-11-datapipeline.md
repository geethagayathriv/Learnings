---
title: "What is Data Pipeline?"
date: 2024-08-11
category: 
---

## What exactly is data pipeline?

In large organisations, data is collected from various sources, in various formats, in large amounts. Data pipelines automate a process of collecting, transforming and delivering data making it usable. 

## Broadly speaking, there are 5 stages in a data pipeline

* Collect
* Ingest
* Store
* Compute
* Consume

The order of these stages can shift based on the type of data.

### Collect

In the scenario of a e-commerce giant, data flows in from various sources like Data stores, data streams and apps.

#### Data stores

* MySQL
* PostgreSQL
* Dynamo DB

#### Data Streams

They deal with live user data like user clicks, searches, data from IOT devices.

### Ingestion

Here data gets loaded into data pipeline environment. Apache Kafka, Amazon Kinesis like tools are commonly used for real-time data streaming.
Data from databases is often ingested through batch processing.

### Compute

#### Batch processing

This involves processing of large data at scheduled intervals. Tools: Apache Hive, Apache Hadoop Map reduce, Apache spark.

#### Stream processing

This handles live data, Tools: Apache flink, Google Dataflow, Apache Storm, Apache Samza.
For example, Apache Flink can be used to identify fradulent transactions by applying critical stream processing rules to the transaction stream.
Stream processing tools directly process data from data stores, data streams and apps rather than tapping into data lakes.

#### ETL or ELT processes

* Extract
* Transform
* Load
Tools: Apache Airflow, AWS Glow
These tools perform extraction of data from data sources, apply transformations and loading the data into the storage layer.

### Store

* Data Lake
* Data warehouse
* Data lakehouse

#### Data Lake

Stores raw, uses tools like HDFS(Hadoop distributed file system), Amazon S3

#### Data Warehouses

Stores structured data, uses tools like Snowflake, Amazon Redshift, Google BigQuery

### Consume

Various end-users leverage this data.
* Data science teams use it for predictive modelling
* BI tools like Tableau r PowerBI provide dashboards and reports.
These tools connect with data warehouses or lakehouses and enable business leaders to visualize KPIs and trends.
* Self-Service analytics tools like Looker empower teams to run queries without deep technical knowledge. 
* ML models use this data for continuous learning and improvement.