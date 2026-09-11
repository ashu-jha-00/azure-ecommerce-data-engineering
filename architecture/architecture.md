                       DATA SOURCE
                      HTTP / REST API
                            │
                            ▼
                ┌──────────────────────┐
                │   Azure Data Factory │
                │       Ingestion      │
                └──────────┬───────────┘
                           │
                           ▼
              ┌─────────────────────────┐
              │       ADLS Gen2         │
              │                         │
              │        BRONZE           │
              │      Raw Data           │
              └────────────┬────────────┘
                           │
                           ▼
                 ┌─────────────────┐
                 │    Databricks   │
                 │     PySpark     │
                 │  Transformation │
                 └────────┬────────┘
                          │
                          ▼
              ┌─────────────────────────┐
              │       ADLS Gen2         │
              │                         │
              │        SILVER           │
              │       Parquet           │
              └────────────┬────────────┘
                           │
                           ▼
                ┌────────────────────┐
                │ Azure Synapse      │
                │ SQL Serving Layer  │
                └──────────┬─────────┘
                           │
                           ▼
                     ┌──────────┐
                     │ Power BI │
                     │ Reports  │
                     └──────────┘