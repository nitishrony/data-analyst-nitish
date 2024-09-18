# Data Analytic Platform for Academics Office

## Project Overview
This project involves developing a comprehensive data analytics platform for the Academics Office using AWS services. The platform manages academic data, including attendance records, through a robust ETL pipeline, data governance, and visualization framework. The goal is to improve data processing, ensure data quality, and provide valuable insights using AWS tools like Amazon S3, AWS Glue, and Amazon QuickSight.

## Objective
The primary objective is to create a secure, scalable, and efficient data analytics platform that supports data ingestion, processing, governance, and visualization for academic datasets in the Academics Office. This platform emphasizes data quality, security, and accessibility to facilitate data-driven decision-making.

## Methodology

### 1. Data Ingestion and Storage
- **Amazon S3 Buckets:**
  - **Landing Bucket:** Stores raw data as it is ingested from various sources.
  - **Raw Bucket:** Contains data after initial cleaning and structuring.
  - **Trusted Bucket:** Holds data that has passed quality checks and validation processes.
  - **Curated Bucket:** Contains fully processed and validated datasets ready for analysis.
  
- **Bucket Structure:**
  - **Attendance/Landing**
  - **Attendance/Raw**
  - **Attendance/Trusted**
  - **Attendance/Curated**
  - **Attendance/Data/Curated/Data Products**

### 2. Data Processing
- **AWS Glue DataBrew and AWS Glue:**
  - **Glue DataBrew:** Used for data profiling, initial cleaning, and transformation tasks.
  - **AWS Glue:** Set up ETL jobs to automate data processing workflows, transforming raw data into trusted and curated datasets.

- **ETL Pipelines:**
  - **Pipeline: Academics Office - Landing to Raw:** Processes initial raw data for basic cleaning.
  - **Pipeline: Trusted to Curated:** Ensures only high-quality data is moved into the curated stage for analysis.

### 3. Data Governance
- **AWS Glue Data Catalog:**
  - Implemented AWS Glue Data Catalog to manage and maintain metadata for the datasets, facilitating easier data discovery and compliance with data governance policies.

- **Security with AWS KMS and IAM:**
  - **AWS Key Management Service (KMS):** Used for encrypting data stored in S3, ensuring data is protected at rest.
  - **AWS Identity and Access Management (IAM):** Configured access controls to ensure only authorized users have access to data and services.

### 4. Data Analysis and Visualization
- **Amazon Athena:**
  - Used Amazon Athena for querying curated datasets directly from S3, enabling quick insights without complex data infrastructure.

- **Amazon QuickSight:**
  - Developed interactive dashboards in Amazon QuickSight to visualize key insights from the academic datasets, allowing stakeholders to explore data trends and patterns.

### 5. Data Monitoring
- **Amazon CloudWatch:**
  - Configured CloudWatch to monitor platform metrics such as storage usage, performance, and costs. Alerts were set up to notify the team of any anomalies or thresholds being breached, such as exceeding budget limits.

### 6. Data Publishing
- **Amazon EC2:**
  - Deployed General and Web Servers on Amazon EC2 instances to facilitate the internal and external sharing of data products and dashboards.

## Tools and Technologies
- **AWS S3:** For secure, scalable data storage across different stages of processing.
- **AWS Glue and Glue DataBrew:** For data preparation, transformation, ETL pipeline management, and data profiling.
- **AWS Athena:** For serverless querying and analysis of datasets stored in S3.
- **Amazon QuickSight:** For creating interactive dashboards and visualizing data insights.
- **AWS KMS:** For encryption and security of sensitive data.
- **Amazon CloudWatch:** For monitoring platform metrics, setting up alerts, and managing operational insights.
- **Amazon EC2:** For hosting and publishing data and dashboards securely.

## Deliverables
- A secure, fully operational data analytics platform with structured data storage and automated data governance.
- ETL pipelines that ensure data quality and facilitate the transformation from raw to curated datasets.
- Interactive dashboards and visualizations in Amazon QuickSight, providing actionable insights for stakeholders.
- A comprehensive data catalog with metadata management for all datasets.
- Continuous monitoring with CloudWatch, including alerts for cost management and operational anomalies.

## Conclusion
The Data Analytic Platform for the Academics Office effectively leverages AWS services to provide a robust framework for managing large-scale academic data. With a focus on security, data quality, and usability, the platform enables the Academics Office to make informed decisions based on reliable and well-governed data.

## Author
- **Nitish Rony**  
