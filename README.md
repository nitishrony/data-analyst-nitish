# Data Analytic Platform for Academics Office

## Project Overview
This project aims to build a comprehensive data analytics platform for the Academics Office using AWS services. The platform manages academic data, including attendance and admissions, through robust ETL pipelines, data governance, and secure data handling mechanisms. It leverages AWS tools such as Amazon S3, AWS Glue, and Amazon QuickSight to ensure data quality, privacy, and accessibility.

## Objective
The primary goal is to create a secure, scalable, and efficient data analytics platform that supports data ingestion, processing, governance, and visualization for academic datasets. This platform focuses on ensuring data quality, protecting sensitive information, and providing valuable insights through visualizations.

## Methodology

### 1. Data Ingestion and Storage
- **Amazon S3 Buckets:**  
  - **Landing Bucket:** Stores raw data as it is ingested from various sources.
  - **Raw Bucket:** Contains data after initial cleaning and structuring.
  - **Trusted Bucket:** Holds data that has passed quality checks and validation processes.
  - **Curated Bucket:** Contains fully processed and high-quality datasets ready for analysis and reporting.
  - ![Screenshot 2024-07-16 160447](https://github.com/user-attachments/assets/61295c87-faa9-4439-9c82-8798b094e661)

  
- **Bucket Structure:**  
  Data is organized in a hierarchical structure across S3 buckets, facilitating efficient data processing and management:
  - **Attendance/Landing**
  - **Attendance/Raw**
  - **Attendance/Trusted**
  - **Attendance/Curated**
  - 
  
### 2. Data Processing
- **AWS Glue DataBrew and AWS Glue:**  
  - Utilized Glue DataBrew for data profiling, initial cleaning, and transformation tasks.
  - Set up AWS Glue ETL jobs to automate data processing workflows, transforming raw data into trusted and curated datasets.

- **ETL Pipelines:**  
  Designed ETL pipelines to streamline data processing:
  - **Pipeline: Academics Office - Landing to Raw:** Processes initial raw data for basic cleaning.
  - **Pipeline: Trusted to Curated:** Ensures only high-quality data is moved into the curated stage for analysis.

### 3. Data Governance
- **Data Catalog:**  
  Implemented AWS Glue Data Catalog to maintain and manage metadata for all datasets. This allows for easier data discovery, tracking, and ensures compliance with data governance policies.

- **Security with KMS and IAM:**  
  - Used AWS Key Management Service (KMS) to encrypt data stored in S3, ensuring secure data at rest.
  - Configured AWS Identity and Access Management (IAM) policies to control access to data and services, enhancing security and compliance.

### 4. Data Analysis and Visualization
- **Amazon Athena:**  
  Used Amazon Athena for querying curated datasets directly from S3, providing quick insights without the need for complex infrastructure.

- **Amazon QuickSight:**  
  Developed interactive dashboards in Amazon QuickSight to visualize key insights from the academic datasets, allowing stakeholders to explore data trends and patterns.

### 5. Data Monitoring
- **Amazon CloudWatch:**  
  Configured CloudWatch to monitor platform metrics such as storage usage, performance, and costs. Set up alerts to notify the team of any anomalies or thresholds being breached, such as exceeding budget limits.

### 6. Data Publishing
- **Amazon EC2:**  
  Deployed a General Server and Web Server on Amazon EC2 instances to facilitate internal and external sharing of data products and dashboards.
  
- **Data Products:**  
  Curated datasets and analytics dashboards were published on web servers, allowing secure access for authorized users to interact with the data products.

## Tools and Technologies
- **AWS S3:** For secure, scalable data storage across various stages of data processing.
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
