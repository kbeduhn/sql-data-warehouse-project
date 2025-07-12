# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! From the development of a data warehouse to the generation of actionable insights, this comprehensive data warehousing and analytics solution showcases industry best practices in data engineering and analytics. 

## Project Overview
This project involves:
1. **Data Architecture:** Designing a Modern Data Warehouse using Medallion Architecture: Bronze, Silver, and Gold layers.
2. **ETL Pipelines:** Extracting, transforming, and loading data from source systems into the data warehouse.
3. **Data Modeling:** Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting:** Creating SQL-based reports and dashboards for actionable insights.

This repository showcases expertise in:
- SQL Development
- Data Architecture
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics

## Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective

Develop a modern data warehouse using SQL Server to consolidate sales data and enable analytical reporting and informed decision-making. 

#### Specifications 

- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality** Clean and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

### BI: Analytics & Reporting (Data Analytics)

#### Objective

Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower key stakeholders with essential business metrics and enable strategic decision-making.

## Data Architecture
The data architecture for this project follows Medallion Architecture Bronze, Silver, and Gold layers:
<img width="1135" height="756" alt="image" src="https://github.com/user-attachments/assets/a4daffb8-dc05-4e45-b282-b2a5e87fdb7c" />

1. **Bronze Layer:** Stores raw data as-is from the source systems. Data is ingested from CSV files into SQL Server Database.
2. **Silver Layer:** This layer includes data cleaning, standardization, and normalization processes to prepare data from analysis.
3. **Gold Layer:** Houses business-ready data modeled into a star schema required for reporting and analytics.

## Repository Structure

data-warehouse-project/
|
|-- datasets/                              # Raw datasets used for the project (ERP and CRM data)
|
|--docs/                                   # Project documentation and architecture details
|-- data_architecture.drawio               # Draw.io file shows the project's architecture
|-- data_catalog.md                        # Catalog of datasets, including the field descriptions and metadata
|-- data_flow.drawio                       # Draw.io file for the data flow diagram
|-- data_models.drawio                     # Draw.io file for data models (star schema)
|-- naming-conventions.md                  # Consistent naming guidelines for tables, columns, and files
|
|-- scripts/                               # SQL scripts for ETL and transformations
|  |--bronze/                              # Scripts for extracting and loading raw data
|  |--silver/                              # Scripts for cleaning and transforming data
|  |--gold/                                # Scripts for creating analytical models
|
|-- tests/                                 # Test scripts and quality files
|
|-- README.md                              # Project overview and instructions
|-- LICENSE                                # License information for the repository
|-- .gitignore                             # Files and directories to be ignored by Git
|-- requirements.tx                        # Dependencies and requirements for the project

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/) You are free to use, modify, and share this project with proper attribution. 
