# AWS Data Analytical Platform for the City of Vancouver
## Project Overview
This project focuses on designing and implementing an AWS Data Analytical Platform (DAP) for processing and analyzing business license data in the City of Vancouver. The project involves setting up scalable, secure, and efficient data pipelines using AWS services like S3, Glue, IAM, KMS, CloudWatch, and CloudTrail. The platform uses these services to handle data ingestion, processing, governance, and real-time monitoring for compelling insights.
## Objective
This project aims to design a robust data platform capable of efficiently processing, cleaning, and analyzing business license data for Vancouver, BC. This project seeks to explore trends, fees, and the issuance of licenses using AWS services to ensure secure, scalable, and cost-effective operations.
Objectives
Data Protection & Governance: Use AWS IAM, KMS, and Glue for access control, encryption, and data governance.

Data Analysis: Conduct descriptive and diagnostic analyses of business licenses to uncover trends and insights.

Data Monitoring: Cost and performance monitoring will be implemented using AWS CloudWatch and CloudTrail.

Performance and Cost Optimization: Achieve operational excellence, security, reliability, and sustainability using AWS services.

## Tools and Technologies
AWS S3: For storing raw, processed, and analyzed data.
AWS Glue: This is used to create ETL pipelines, transform data, and govern governance.
AWS Athena: This is used to query and analyze data directly from S3.
AWS IAM: For managing secure access to AWS resources.
AWS KMS: This is for encrypting data at rest and in transit.
AWS CloudWatch: This is used to monitor system performance and cost management.
AWS CloudTrail: This is for logging and tracking API activities.
EC2: For deploying data visualizations and reports.
# Project Structure
Reports
The project has two key reports, each outlining specific aspects of the AWS platform’s design, security, and analysis:
## Part 1 Report: Data Analytical Platform Design
It covers the architecture, data ingestion methods, and steps to process and analyze business license data.

## Part 2 Report: AWS Security, Governance, and Monitoring
Highlights AWS’s security, data governance, and real-time monitoring services, focusing on how IAM, KMS, Glue, and CloudWatch are integrated for this project.

## Datasets
The following datasets, consisting of business license data from 2023 and 2024, were used to demonstrate data cleaning, ingestion, and analysis:

Business Licenses 2023
Business Licenses 2024

These datasets were ingested into AWS S3 and processed using AWS Glue for further analysis in Athena.

## Scripts
Python scripts were used to clean and process the business license data. These scripts can be adapted for other datasets or ETL processes.

## Data Processing Script
Demonstrates how to clean and process business license data using Python and AWS Glue.
Architecture
The project’s architecture diagram illustrates how AWS services were integrated to handle the data pipeline from ingestion to analysis, including security and monitoring features.

## Architecture Diagram
This diagram visualizes the data flow through AWS services, showing key elements like IAM, S3, Glue, CloudWatch, and EC2.

## Methodology
### 1. Data Collection
Source: Data was sourced from the City of Vancouver’s open data portal, focusing on business license data for 2023 and 2024.

<img width="1199" alt="Screenshot 2024-08-27 at 3 11 47 PM" src="https://github.com/user-attachments/assets/4516cffe-59b1-4069-b77a-2a1ba6eaf692">


<img width="814" alt="Screenshot 2024-08-27 at 3 09 59 PM" src="https://github.com/user-attachments/assets/915238c2-669d-47e5-aab0-b288946eae84">


### 2. Data Ingestion
The raw data was stored in AWS S3, with separate folders for 2023 and 2024 business license data.

<img width="452" alt="image" src="https://github.com/user-attachments/assets/ce9c489e-e10a-45cf-93d6-389a79d7493a">A detailed explanation of the data storage design includes.

Landing Folder: Stores the raw operational data.
Raw Folder: Stores cleaned and restructured data.

<img width="452" alt="image" src="https://github.com/user-attachments/assets/180ba245-a7df-429a-8f44-94d0477bd4d7">

<img width="452" alt="image" src="https://github.com/user-attachments/assets/825ff032-117d-4705-85ea-9fb11271652f">

Curated Folder: Stores analyzed data after ETL processing.
Ingestion Process: 
Upload of Operational data from the City of Vancouver portal in Excel format in Landing folders of 2023 and 2024, respectively:

### 4. Data Processing
Data cleaning and restructuring were handled using AWS Glue. Glue’s Databrew was used to automate ETL (Extract, Transform, Load) processes.
Data was then analyzed using AWS Athena, providing insights into business trends, average license fees, and more.

<img width="454" alt="image" src="https://github.com/user-attachments/assets/fac7ee76-e28b-4d86-a64e-792d5ad4c5f2">


<img width="194" alt="image" src="https://github.com/user-attachments/assets/2f94533d-49b1-4e22-b394-09e67eb4f6dc">

### 5. Data Governance & Security
IAM and KMS were employed to enforce access control and data encryption. Sensitive data was protected using KMS encryption both at rest and in transit.
AWS Glue handled data governance, ensuring data quality and compliance with pre-defined policies.


### 6. Data Monitoring
AWS CloudWatch provides real-time monitoring of resource usage and costs.
CloudTrail tracked API activities, logging data access and changes to ensure full transparency.
## Key Features
### Data Security: 
AWS IAM and KMS were used to control access and ensure the security of sensitive data.
### Data Governance: 
AWS Glue automated data cleaning and monitoring, ensuring that only relevant, compliant data was processed.
### Data Monitoring: 
AWS CloudWatch and CloudTrail provided real-time monitoring and cost management, with alarms configured to track unexpected changes in usage.


## View Results in AWS Athena:
Use AWS Athena to query and analyze the cleaned data stored in your S3 bucket. You can create SQL queries to extract insights into business license trends and fees.

## Deliverables
1. Detailed descriptions of the project’s design, implementation, and AWS services used.
2. Data Storage and Ingestion: S3 bucket structure and data ingestion pipeline.
3. Data Cleaning & Preparation: AWS Glue scripts for cleaning and restructuring.

<img width="452" alt="image" src="https://github.com/user-attachments/assets/6a6ca1ac-2730-4320-9c53-50f18b29c183">

4. ETL Pipeline: Complete AWS Glue ETL pipeline for business license data.

<img width="452" alt="image" src="https://github.com/user-attachments/assets/1562b6a2-3b19-46bb-89df-657244cc1966">

5. Data Analysis & Visualization: Query results from AWS Athena and visual reports.
 
  <img width="454" alt="image" src="https://github.com/user-attachments/assets/23eb4b1e-8f54-497c-8bce-e3212bb35704">

6. Monitoring & Cost Management: CloudWatch dashboard and cost alarms.

7. Security: IAM roles and KMS encryption policies.


## Sample Datasets:
Cleaned and processed datasets from 2023 and 2024 for analysis in AWS Athena.

## Scripts:
Python scripts for processing and cleaning business license data, ready to be integrated with AWS Glue pipelines.

## Architecture Diagram:
A visual guide to the AWS services used in the project, highlighting how they interact and handle different parts of the data pipeline.

## Conclusion
The AWS Data Analytical Platform for the City of Vancouver offers a scalable, secure, and efficient solution for processing business license data. The platform ensures high operational excellence, security, and cost efficiency by integrating AWS services such as S3, Glue, IAM, and CloudWatch. The insights generated from this data can be used to inform policy decisions and improve the management of business licenses in Vancouver.
