# PySpark-dbt-End-to-End-Data-Engineering-Project-Building-an-Uber-Analytics-Platform


## Project Overview

This project demonstrates an End-to-End Data Engineering Pipeline built using Databricks, PySpark, Delta Lake, and dbt following the Medallion Architecture (Bronze → Silver → Gold).

The pipeline ingests raw taxi transportation data into Databricks Bronze tables, performs cleansing and standardization in the Silver layer using PySpark, and then applies business transformations and dimensional modeling in dbt to create Gold-layer analytical datasets.

The final Gold tables are materialized back into Databricks and are ready for reporting, dashboarding, and business intelligence use cases.

---

## Architecture

Source Data
↓
Bronze Layer (Raw Data)
↓
Silver Layer (Cleaned Data)
↓
dbt Transformations
↓
Gold Layer (Star Schema)
↓
Databricks Gold Tables


---

## Technology Stack

* Databricks
* PySpark
* Delta Lake
* dbt Cloud
* SQL
* GitHub
* Star Schema Modeling

---

## Medallion Architecture

### Bronze Layer

Raw data ingestion layer containing:

* customers
* drivers
* locations
* payments
* trips
* vehicles

Purpose:

* Store source data
* Preserve raw records
* Support data lineage

---

### Silver Layer

Data cleansing and transformation layer.

Operations Performed:

* Data cleaning
* Null handling
* Data type standardization
* Deduplication
* Business rule validation

Tables:

* customers
* drivers
* locations
* payments
* trips
* vehicles

---

### Gold Layer

Business-ready analytical layer built using dbt.

Dimension Tables:

* dimcustomers
* dimdrivers
* dimlocations
* dimpayments
* dimvehicles

Fact Table:

* facttrips

Purpose:

* Reporting
* KPI Calculation
* Business Intelligence
* Dashboarding

---

## Data Model

The Gold Layer follows a Star Schema design.

Fact Table:

* facttrips

Dimension Tables:

* dimcustomers
* dimdrivers
* dimlocations
* dimpayments
* dimvehicles

---

## dbt Features Used

* Sources
* Models
* Snapshots
* Tests
* Documentation
* SQL Transformations

Files:

* sources.yml
* trips.sql
* fact.yml
* scd.yml

---

## Data Quality Checks

Implemented through dbt tests:

* Unique Key Validation
* Not Null Validation
* Referential Integrity
* Relationship Testing

---

## Project Workflow

1. Load source data into Bronze tables.
2. Transform and clean data into Silver tables using PySpark.
3. Use dbt to create Gold-layer business models.
4. Generate dimension and fact tables.
5. Materialize Gold tables back into Databricks.
6. Use Gold tables for analytics and reporting.

---

## Business Value

This project demonstrates:

* Modern Data Engineering Practices
* ELT Architecture
* Medallion Architecture
* Data Modeling
* Analytics Engineering
* Data Quality Management
* Scalable Data Pipelines

---

## Skills Demonstrated

* Databricks
* PySpark
* SQL
* dbt
* Delta Lake
* Data Warehousing
* Data Modeling
* Data Quality Testing
* Git & GitHub

---

## 🛠️ Tech Stack



## 🔄 CI/CD Pipeline

[![dbt CI/CD](https://github.com/yourusername/databricks-dbt-medallion-pipeline/actions/workflows/dbt-ci.yml/badge.svg)](https://github.com/yourusername/databricks-dbt-medallion-pipeline/actions/workflows/dbt-ci.yml)

![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
Data Engineer | Analytics Engineer | Python Developer
