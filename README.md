# sql-data-warehouse-ssas-analytics
End-to-end data warehouse, exploratory analytics, advanced SQL analysis, and SSAS Tabular semantic modeling project
# SQL Server Data Warehouse & SSAS Sales Analytics

An end-to-end data analytics project built using Microsoft SQL Server, covering
data warehousing, ETL, Medallion Architecture, Star Schema, Exploratory Data
Analysis, Advanced Analytics, business reporting, and SSAS Tabular semantic modeling.

---

## Project Overview

This project demonstrates an end-to-end data pipeline that transforms raw CRM
and ERP CSV data into trusted analytical data and business-ready insights.

The project is divided into two major analytical stages:

1. SQL Server Data Warehouse
2. EDA & Advanced Data Analytics

The project is now being extended with an SSAS Tabular semantic layer to
provide centralized business measures, relationships, hierarchies, and KPIs
for BI consumption.

---

## Architecture

```text
CRM / ERP CSV Files
        |
        v
+------------------+
|  Bronze Layer    |
|  Raw Data        |
+------------------+
        |
        v
+------------------+
|  Silver Layer    |
| Cleaned Data    |
+------------------+
        |
        v
+------------------+
|   Gold Layer     |
|  Star Schema     |
+------------------+
        |
        +--------------------+
        |                    |
        v                    v
      EDA              Advanced Analytics
        |                    |
        +---------+----------+
                  |
                  v
          Reporting Views
                  |
                  v
        +-------------------+
        |   SSAS Tabular    |
        | Semantic Model    |
        +-------------------+
                  |
                  v
          Power BI / Excel
