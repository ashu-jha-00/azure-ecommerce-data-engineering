# Azure End-to-End E-Commerce Data Engineering Project

## 📌 Overview

This project implements an end-to-end Azure data engineering
pipeline for ingesting, transforming, storing and serving
e-commerce data.

## 🏗️ Architecture

HTTP API
   ↓
Azure Data Factory
   ↓
Azure Data Lake Storage Gen2
   ↓
Databricks / PySpark
   ↓
Silver Parquet
   ↓
Azure Synapse Analytics
   ↓
Power BI

## 🛠️ Technologies

- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Databricks
- PySpark
- Azure Synapse Analytics
- SQL
- Power BI

## 🔄 Data Flow

### 1. Ingestion

Azure Data Factory retrieves data from the source
and loads it into the Bronze layer.

### 2. Bronze

Raw data is stored in ADLS Gen2.

### 3. Silver

Databricks performs:

- Data cleansing
- Null handling
- Data type conversion
- Duplicate removal
- Derived columns
- Business transformations

Silver data is stored as Parquet.

### 4. Serving

Azure Synapse Analytics provides the SQL serving layer.

### 5. Reporting

Power BI consumes the curated data for reporting.

## 📂 Repository Structure

...

## 🧪 Data Quality

...

## 📊 Results

...

## 📸 Screenshots

...

## 🚀 Key Learnings

- Azure Data Factory orchestration
- ADLS Gen2 data lake architecture
- PySpark transformations
- Parquet storage
- Synapse SQL
- End-to-end pipeline orchestration
- Azure data engineering architecture