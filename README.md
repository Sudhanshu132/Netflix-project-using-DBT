# Netflix Project Using dbt

This repository contains a **dbt (Data Build Tool)** project that transforms raw Netflix dataset files into analytics-ready models using a layered ELT approach.  
The project demonstrates best practices in dbt modeling, data testing, and documentation.

---

## 🧠 Project Overview

This project builds a complete **ELT pipeline** to convert raw Netflix data into structured tables and facts usable for analytics and reporting.  
It uses dbt to manage SQL transformations, enforce data quality, and produce clean data for downstream BI tools.

---

## 📦 Tech Stack

- **dbt** – Transform data and build models  
- **SQL** – SQL logic and business rules  
- **GitHub** – Version control  
- **Cloud Warehouse** (optional) – e.g., Snowflake / BigQuery / Synapse

---

## 🚀 Key Features

- Staging, intermediate, and mart layers for clean modeling
- dbt tests (not_null, unique, relationships) to enforce data quality
- Configurable incremental models for efficient processing
- Documentation enabled for data lineage and model context

---

## 📁 Repository Structure

├── models/  //
│ ├── staging/ # Source cleaning and typing
│ ├── intermediate/ # Business logic transformations
│ └── marts/ # Final fact & dimension tables
├── snapshots/ # Slowly changing dimensions (optional)
├── macros/ # Reusable SQL snippets
├── dbt_project.yml # dbt project config
└── profiles.yml # dbt connection settings


---

## 🛠 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Sudhanshu132/Netflix-project-using-DBT.git
cd Netflix-project-using-DBT

pip install dbt


dbt debug
dbt run
dbt test
dbt docs generate
dbt docs serve

