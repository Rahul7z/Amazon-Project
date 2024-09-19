
# AWS Data Analytical Platform for the City of Vancouver

# Project Description
This project focuses on designing and implementing a Data Analytical Platform (DAP) for the City of Vancouver using AWS services. The platform aims to streamline data ingestion, storage, and analysis, providing insights across various domains, including Business and Economy. By leveraging AWS S3, Glue, and Athena, the platform handles datasets from 2013 to 2024 business licenses to offer valuable descriptive analysis.

# Objective
The objective is to build a scalable and efficient data analytical platform using AWS that can handle large datasets, provide clean and restructured data, and generate insightful analyses. Specifically, the project aims to understand trends in business license issuance, analyze fees, and generate insights for policymakers and business operators in Vancouver.

# Dataset
The primary dataset includes business license data from 2013 to 2024 for the province of British Columbia, particularly focusing on the years 2023 and 2024. The data was sourced from the City of Vancouver's open data portal and includes fields such as business type, license fees, issue date, and expiry date.

Link to dataset: Business Licenses 2013-2024

# Methodology
## Data Collection and Preparation:

Data was sourced from the City of Vancouver's open data portal.
Files were cleaned using AWS Glue Databrew to remove missing values and reformat columns.
Dataset restructuring involved the addition of derived columns and data-type changes.
Data Storage Design:

Data was stored in an AWS S3 bucket with folders for "Landing" (raw data), "Raw" (processed data), and "Curated" (analyzed data).
Folders were created for both the 2023 and 2024 datasets.
## Data Pipeline Implementation:

## ETL (Extract, Transform, Load) processes were managed using AWS Glue.
The pipeline involved schema changes, union operations for combining datasets, and aggregate functions to compute metrics like the average fee paid for licenses.
Data Analysis and Visualization:

## Data was analyzed in AWS Athena, with a custom table created to store processed data.
Data was visualized using tools like AWS Quicksight and Matplotlib for insights into business license trends.
Data Publishing:

## The analyzed data was published on an EC2 instance configured as a web server, accessible via a public IP.
Tools and Technologies
Data Storage & Processing: AWS S3, AWS Glue
Data Cleaning & Restructuring: AWS Glue Databrew
Data Analysis: AWS Athena
Visualization: AWS Quicksight, Python (Matplotlib)
Publishing: EC2 (Web Server)
# Deliverables
A cleaned and restructured dataset for business licenses from 2023 and 2024.
An ETL pipeline designed using AWS Glue to ingest and process data.
Visualizations of business license trends in British Columbia.
A final report summarizing key insights and analysis results.
A published web server with access to analysis results.


