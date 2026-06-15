# retail_sales_data_etl_automation
Power Query ETL automation in Excel built to transform raw retail sales exports into reporting ready datasets for weekly business reporting.

## 1. Project Background

The Textile (TXT) Department relied on a manual weekly reporting process based on Excel VLOOKUPs, file merges and repetitive data preparation tasks.
Every Monday morning, sales data had to be prepared before reporting deadlines. As data volumes increased, the process became difficult to maintain, highly dependent on individual knowledge and increasingly vulnerable to delays or personnel changes.
To address these challenges, a centralized Power Query ETL framework I developed to automate data preparation and provide fast access to reporting ready datasets through a single refresh process.

## 2. Objective

The objective of this project was to build a reusable Power Query ETL framework capable of supporting multiple textile departments through a common transformation architecture.

The framework was designed to:

* Standardize weekly sales data preparation.
* Centralize transformation logic within a single workflow.
* Replace manual VLOOKUP based data enrichment processes.
* Integrate supplementary business datasets and lookup tables.
* Automate product, store and assortment mapping.
* Reduce dependency on individual employees.
* Simplify onboarding and future maintenance.
* Ensure consistent reporting structures across departments.
* Provide a scalable foundation for future reporting and automation initiatives.

## 3. Architecture Overview

The solution is built around a centralized Power Query ETL framework designed to automate weekly retail data preparation.
All transformation logic is maintained within a single Excel workbook, while source files and supplementary reference datasets are stored separately. This architecture allows business users to replace source files and refresh the entire workflow without modifying transformation logic.

## Project Structure

```
retail-sales-data-etl-automation/
│
├── weekly_data_etl.xlsx
│
├── data/
│   └── data.xlsx
│
└── supplementary/
    └── supplementary.xlsx
```
## Architecture Flow

```
Sales Data Exports
      │
      ▼
Power Query ETL
      ├── Data Validation
      ├── Data Standardization
      ├── Data Enrichment
      ├── Store Mapping
      ├── Business Rules
      ▼
      Reporting Ready Dataset
```
