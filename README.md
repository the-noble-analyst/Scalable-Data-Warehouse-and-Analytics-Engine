# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:
![Data Architecture](docs/data_architecture.png)

1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.
5. **Data Visualisation**: Develop an interactive Power BI dashboard to visualize key business metrics and trends, enabling stakeholders to explore data insights through intuitive visual analytics.


🎯 This repository is an excellent resource for professionals and students looking to showcase expertise in:
- SQL Development
- Data Architect
- Data Engineering  
- ETL Pipeline Developer  
- Data Modeling  
- Data Analytics
- Data Visualisation

---

## 🛠️ Important Links & Tools:

Everything is for Free!
- **[Datasets](datasets/):** Access to the project dataset (csv files).
- **[SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads):** Lightweight server for hosting your SQL database.
- **[SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16):** GUI for managing and interacting with databases.
- **[Git Repository](https://github.com/):** Set up a GitHub account and repository to manage, version, and collaborate on your code efficiently.
- **[DrawIO](https://www.drawio.com/):** Design data architecture, models, flows, and diagrams.
---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

These insights empower stakeholders with key business metrics, enabling strategic decision-making.  

## 📂 Repository Structure
```
data-warehouse-project/
│
├── Data visualisation/                 # visualize key business metrics and trends
│   ├── Power BI Report.png             
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)    
│                     
│   ├── source_crm/
│       ├──cust_info.csv
│       ├── prd_info.csv
│       ├──sales_details.csv
│   ├── source_erp/
│       ├── CUST_AZ12.csv
│       ├── LOC_A101.csv
│       ├── PX_CAT_G1V2.csv                        
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.png                         # file shows all different techniquies and methods of ETL
│   ├── data_architecture.png           # file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.png                   # file for the data flow diagram
│   ├── data_model.png                  # file for data models (star schema)
|   ├── data_integration                # how tables are related
│   ├── naming_conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── exploratory_data_analysis/
│   ├──00_init_database.sql
│   ├──01_database_exploration.sql
│   ├──02_dimensions_exploration.sql
│   ├──03_date_range_exploration.sql
│   ├──04_measures_exploration.sql
│   ├──05_magnitude_analysis.sql
│   ├──06_ranking_analysis.sql
│   ├──07_change_over_time_analysis.sql
│   ├──08_cumulative_analysis.sql
│   ├──09_performance_analysis.sql
│   ├──10_data_segmentation.sql
│   ├──11_part_to_whole_analysis.sql
│   ├──12_report_customers.sql
│   ├──13_report_products.sql
│  
├── scripts/                            # SQL scripts for ETL and transformations
│         ├── bronze/                         # Scripts for extracting and loading raw data
│                  ├── ddl_bronze.sql
│                  ├── proc_load_bronze.sql
│
│         ├── silver/                         # Scripts for cleaning and transforming data
│                   ├── ddl_silver.sql
│                   ├── proc_load_silver.sql   
│         ├── gold/                           # Scripts for creating analytical models
│                   ├──ddl_gold.sql
│          ── init_database.sql
├── tests/                              # Test scripts and quality files
│       ├── quality_checks_gold.sql
│       ├── quality_checks_silver.sql
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository
```
---
---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.
