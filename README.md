# Riyadh Metro Data Engineering Platform

An end-to-end data engineering platform for Riyadh Metro operations, built using Microsoft Fabric, PySpark, SQL, real-time streaming, data pipelines, data warehousing, and Power BI.

## Project Overview

This project demonstrates an end-to-end data engineering workflow for Riyadh Metro operational data.
The platform combines batch data processing, data transformation, real-time streaming, data warehousing, security, and Power BI to support operational monitoring and decision support.

## Architecture

The project follows a layered data engineering architecture:
**Sources → Bronze → Silver → Gold → Data Warehouse → Power BI
The project also includes a real-time streaming flow:
**Smart Metro Simulator → Eventstream → Eventhouse → Real-Time Analytics

## Technologies

- Microsoft Fabric
- OneLake
- Lakehouse
- PySpark
- Python
- SQL
- Apache Spark
- Data Pipelines
- Eventstream
- Eventhouse
- KQL
- Data Warehouse
- Power BI
- Git & GitHub

## Data Engineering Layers

### Bronze Layer

The Bronze layer contains ingested data including:

- Metro stations
- Metro lines
- Events
- Trips
- Weather

### Silver Layer

The Silver layer contains cleaned and transformed data prepared for further processing and analytical use.
### Gold Layer

The Gold layer contains curated datasets prepared for downstream analytical and business use.

## Data Warehouse

The project includes a structured data warehouse containing dimension and fact tables for Riyadh Metro operations.
Key warehouse objects include:

- 'dim_lines'
- 'dim_stations'
- 'dim_events'
- 'dim_weather'
- 'fact_trips'
- 'metro_line_paths'
- 'UserStationAccess'

## Real-Time Streaming

A Smart Metro Simulator generates simulated metro events continuously.
The streaming data is processed through Microsoft Fabric Eventstream and stored in Eventhouse for real-time analysis.

## Data Security

The project includes access-control and data-masking concepts.
'UserStationAccess' is used to support station-level access control, while sensitive passenger-related information is protected through data masking.
## Power BI Dashboard

The final Power BI dashboard provides an operational overview of Riyadh Metro data.
The dashboard includes:

- Total trips
- Completed trips
- Operational metrics
- Metro line selection
- Date filtering
- Time filtering
- Riyadh Metro map visualization

## Project Structure
'''text
Riyadh Metro Data
│
├── notebooks
│   ├── bronze
│   ├── silver
│   ├── gold
│   ├── realtime
│   └── metro_line_paths.ipynb
│
├── SQL
│   └── SQL scripts
│
├── pipeline
│   ├── manifest
│   └── pipeline
│
├── architecture
│   └── architecture image
│
└── README.md


## Objective

The objective of this project is to demonstrate practical data engineering skills through a Microsoft Fabric solution covering:

- Batch data processing
- ELT data transformation
- Data pipelines
- Lakehouse architecture
- PySpark processing
- Data warehousing
- Real-time streaming
- Data security
- Power BI visualization

## Data Sources

The project uses a combination of real source data, API-based data, and simulated/streaming data to demonstrate different data engineering scenarios.

## Project Outcome

This project demonstrates the implementation of a complete data engineering platform from data ingestion and transformation to data warehousing, real-time processing, security, and business intelligence.