# retail_sales_data_etl_automation
Power Query ETL automation in Excel built to transform raw retail sales exports into reporting ready datasets for weekly business reporting.

## 1. Business Problem

The Textile (TXT) Department relied on a manual weekly preparing data for reporting process based on Excel VLOOKUPs, multiple source files and repetitive data preparation tasks.
Every Monday, sales data had to be manually consolidated, validated and enriched before reporting deadlines. As data volumes increased, the process became increasingly time consuming, difficult to maintain and highly dependent on individual knowledge.
To address these challenges, I developed a reusable Power Query ETL solution that standardized data preparation, automated transformation logic and created a common reporting structure that could be deployed across multiple departments.

## 2. Solution Overview

To eliminate manual reporting preparation, I designed and developed a centralized Power Query ETL framework within Excel 2013.
The solution acts as a data preparation layer between raw sales exports and the final reporting process used by the Textile Department. Instead of maintaining hundreds of VLOOKUPs and manual mappings each week a lot hours, all transformation logic was consolidated into a single automated workflow.
Users only need to replace the latest source files and refresh the model. During refresh, the ETL process automatically validates, transforms and enriches the data using supplementary datasets containing store information, coordinator assignments, product hierarchies, seasonal collections, brick classifications, model mappings and other business attributes.
The final output is a standardized and reporting-ready dataset that can be immediately used for operational reporting, KPI analysis and business decision-making.
By centralizing transformation logic into a single workflow, the project significantly reduced manual preparation effort while improving data consistency, maintainability and process continuity across the department.



## 3. Architecture Overview

The project is built around a centralized Power Query ETL architecture designed to standardize weekly sales data preparation across multiple textile departments.
All transformation logic is maintained within a single Excel workbook, while source files and supplementary datasets are stored separately. This approach simplifies maintenance, improves scalability and allows business rules to be managed in one location.
The architecture was designed to support different departments using the same ETL structure while maintaining department specific source files, mappings and business attributes.
Once configured, the process requires only two actions:
Replace source files.
Refresh the workbook.
The ETL workflow then automatically generates a fully standardized and reporting ready dataset.



**Project Structure**

![scheme](./images/scheme.png)



## 4.Business Impact

This project was created to solve a real business problem rather than as a portfolio exercise.
The original reporting process relied on manual Excel work, VLOOKUP-based mappings, repetitive file merges and employee-specific knowledge accumulated over many years. As a result, onboarding new team members was difficult, reporting preparation was time-consuming and the process was vulnerable to errors and staff turnover.
By implementing a centralized Power Query ETL workflow, the entire data preparation process was standardized and reduced to a simple refresh operation. Complex transformation logic became embedded within the framework instead of depending on individual Excel skills.
The solution improved reporting consistency, reduced manual effort and created a repeatable process that could be easily maintained and transferred across the team.
Why This Project Matters
Although modern BI platforms are becoming increasingly popular, many organizations still rely on manual spreadsheet-based reporting processes.
This project demonstrates how significant operational improvements can be achieved using tools already available in many companies. In this case, Excel 2013 combined with the Power Query add-in was sufficient to transform a long-standing manual workflow into a structured ETL process.
The goal of this repository is not to showcase a complex technology stack, but to demonstrate how practical data automation can solve real business problems and deliver measurable value.



