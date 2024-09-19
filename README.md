# AWS Data Analytical Platform for the City of Vancouver
## Project Overview
This project focuses on the design and implementation of an AWS Data Analytical Platform (DAP) for processing and analyzing business license data in the City of Vancouver. The project involves setting up scalable, secure, and efficient data pipelines using AWS services like S3, Glue, IAM, KMS, CloudWatch, and CloudTrail. By leveraging these services, the platform handles data ingestion, processing, governance, and real-time monitoring for effective insights.
<img width="814" alt="Screenshot 2024-08-27 at 3 09 59 PM" src="https://github.com/user-attachments/assets/915238c2-669d-47e5-aab0-b288946eae84">

<img width="1199" alt="Screenshot 2024-08-27 at 3 11 47 PM" src="https://github.com/user-attachments/assets/4516cffe-59b1-4069-b77a-2a1ba6eaf692">


## Objective
The objective of this project is to design a robust data platform capable of efficiently processing, cleaning, and analyzing business license data for Vancouver, BC. This project seeks to explore trends, fees, and the issuance of licenses using AWS services to ensure secure, scalable, and cost-effective operations.

## Tools and Technologies
AWS S3: For storing raw, processed, and analyzed data.
AWS Glue: For creating ETL pipelines, data transformation, and governance.
AWS Athena: For querying and analyzing data directly from S3.
AWS IAM: For managing secure access to AWS resources.
AWS KMS: For encrypting data at rest and in transit.
AWS CloudWatch: For monitoring system performance and cost management.
AWS CloudTrail: For logging and tracking API activities.
EC2: For deploying data visualizations and reports.
Project Structure
Reports
The project has two key reports, each outlining specific aspects of the AWS platform’s design, security, and analysis:

## Part 1 Report: Data Analytical Platform Design
Covers the overall architecture, data ingestion methods, and the steps taken to process and analyze business license data.

Part 2 Report: AWS Security, Governance, and Monitoring
Highlights AWS’s security, data governance, and real-time monitoring services, focusing on how IAM, KMS, Glue, and CloudWatch are integrated for this project.

Datasets
The following datasets, consisting of business licenses data from 2023 and 2024, were used to demonstrate data cleaning, ingestion, and analysis:

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
This diagram visualizes the flow of data through AWS services, showing key elements like IAM, S3, Glue, CloudWatch, and EC2.

## Methodology
1. Data Collection
Source: Data was sourced from the City of Vancouver’s open data portal, focusing on business license data for the years 2023 and 2024.
2. Data Ingestion
The raw data was stored in AWS S3, with separate folders for 2023 and 2024 business licenses data.
A detailed explanation of the data storage design includes:
Landing Folder: Stores the raw operational data.
Raw Folder: Stores cleaned and restructured data.
Curated Folder: Stores analyzed data after ETL processing.
3. Data Processing
Data cleaning and restructuring were handled using AWS Glue. Glue’s Databrew was used to automate ETL (Extract, Transform, Load) processes.
Data was then analyzed using AWS Athena, providing insights into business trends, average license fees, and more.
4. Data Governance & Security
IAM and KMS were employed to enforce access control and data encryption. Sensitive data was protected using KMS encryption both at rest and in transit.
AWS Glue handled data governance, ensuring data quality and compliance with pre-defined policies.
5. Data Monitoring
AWS CloudWatch provided real-time monitoring of resource usage and costs.
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
Reports:
Detailed descriptions of the project’s design, implementation, and AWS services used.

## Sample Datasets:
Cleaned and processed datasets from 2023 and 2024 for analysis in AWS Athena.

Scripts:
Python scripts for processing and cleaning business license data, ready to be integrated with AWS Glue pipelines.

Architecture Diagram:
A visual guide to the AWS services used in the project, highlighting how they interact and handle different parts of the data pipeline.

## Conclusion
The AWS Data Analytical Platform for the City of Vancouver offers a scalable, secure, and efficient solution for processing business license data. By integrating AWS services such as S3, Glue, IAM, and CloudWatch, the platform ensures high standards of operational excellence, security, and cost efficiency. The insights generated from this data can be used to inform policy decisions and improve the management of business licenses in Vancouver.
