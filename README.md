# Data Analytic Platform for Academics Office

## Project Overview
This project involves developing a comprehensive data analytics platform for the Academics Office using AWS services. The platform manages academic data, including attendance records, through a robust ETL pipeline, data governance, and visualization framework. The goal is to improve data processing, ensure data quality, and provide valuable insights using AWS tools like Amazon S3, AWS Glue, and Amazon QuickSight.

## Objective
The primary objective is to create a secure, scalable, and efficient data analytics platform that supports data ingestion, processing, governance, and visualization for academic datasets in the Academics Office. This platform emphasizes data quality, security, and accessibility to facilitate data-driven decision-making.

## Methodology

![image](https://github.com/user-attachments/assets/36c21625-0247-4a26-a7cc-1605c0ea60f0)


### 1. Data Ingestion and Storage
- **Amazon S3 Buckets:**
  - **Landing Bucket:** Stores raw data as it is ingested from various sources.
  - ![AWS implementation result-1](https://github.com/user-attachments/assets/19617e2a-54d2-41bd-bed1-59e822dcf314)
  - ![Screenshot 2024-08-19 095817](https://github.com/user-attachments/assets/75096c67-bc34-40f5-a80b-52f040617c31)


  - **Raw Bucket:** Contains data after initial cleaning and structuring.
 
  - **Curated Bucket:** Contains fully processed and validated datasets ready for analysis.
  - 
  - **Trusted Bucket:** Holds data that has passed quality checks and validation processes.
  - ![Screenshot 2024-08-27 140539](https://github.com/user-attachments/assets/c6271137-c8ce-4743-9fc6-614160bebb47)



  

- **Bucket Structure:**
  - **Attendance/Landing**
  - **Attendance/Raw**
  - **Attendance/Trusted**
  - **Attendance/Curated**
  - **Attendance/Data/Curated/Data Products**

### 2. Data Processing
- **AWS Glue DataBrew and AWS Glue:**
  - **Glue DataBrew:** Used for data profiling, initial cleaning, and transformation tasks.
  - ![Screenshot 2024-07-23 142613](https://github.com/user-attachments/assets/26289c9a-cbcb-4cb9-ab20-92a694caf76d)

  - 
  - **AWS Glue:** Set up ETL jobs to automate data processing workflows, transforming raw data into trusted and curated datasets.
  - ![image](https://github.com/user-attachments/assets/f525a561-bd2d-441e-9f3c-486865fb60a1)


- **ETL Pipelines:**
  - **Pipeline: Academics Office - Landing to Raw:** Processes initial raw data for basic cleaning.
  - **Pipeline: Trusted to Curated:** Ensures only high-quality data is moved into the curated stage for analysis.

### 3. Data Governance
- **AWS Glue Data Catalog:**
  - Implemented AWS Glue Data Catalog to manage and maintain metadata for the datasets, facilitating easier data discovery and compliance with data governance policies.
    ![Screenshot 2024-08-27 140424](https://github.com/user-attachments/assets/8d927fb9-2032-4268-bf30-049ddbedc1f3)
    ![Screenshot 2024-08-27 140625](https://github.com/user-attachments/assets/7ffe5f83-64d7-49da-986c-0d6af9141062)





- **Security with AWS KMS and IAM:**
  - **AWS Key Management Service (KMS):** Used for encrypting data stored in S3, ensuring data is protected at rest.
  - ![Screenshot 2024-08-20 140156](https://github.com/user-attachments/assets/7bd161bd-dda4-4f20-b930-d32ec4cb803d)

  - **AWS Identity and Access Management (IAM):** Configured access controls to ensure only authorized users have access to data and services.
  - ![Screenshot 2024-08-20 140221](https://github.com/user-attachments/assets/767e574d-92ae-4ee8-bb58-dcf917c8db8b)


### 4. Data Analysis and Visualization
- **Amazon Athena:**
  - Used Amazon Athena for querying curated datasets directly from S3, enabling quick insights without complex data infrastructure.
  - ![Screenshot 2024-07-30 135851](https://github.com/user-attachments/assets/c9ed5103-468b-4283-bd96-c761c740f8a5)


- **Amazon QuickSight:**
  - Developed interactive dashboards in Amazon QuickSight to visualize key insights from the academic datasets, allowing stakeholders to explore data trends and patterns.

### 5. Data Monitoring
- **Amazon CloudWatch:**
  - Configured CloudWatch to monitor platform metrics such as storage usage, performance, and costs. Alerts were set up to notify the team of any anomalies or thresholds being breached, such as exceeding budget limits.
  - ![Screenshot 2024-09-03 132701](https://github.com/user-attachments/assets/d67f7653-a57f-4ee6-bc5b-2fe4f1c1e727)
  - ![Screenshot 2024-09-03 134637](https://github.com/user-attachments/assets/a7e11ac0-ac13-4d88-94a4-29a72f52ada1)
  - ![Screenshot 2024-09-03 140144](https://github.com/user-attachments/assets/dbe100cb-7c2b-49a7-9364-2db08973e1b5)




### 6. Data Publishing
- **Amazon EC2:**
  - Deployed General and Web Servers on Amazon EC2 instances to facilitate the internal and external sharing of data products and dashboards.
  - ![Screenshot 2024-08-05 161910](https://github.com/user-attachments/assets/d8b54639-e70a-41a3-85fa-89255754f04f)
  - ![Screenshot 2024-08-05 170712](https://github.com/user-attachments/assets/bcf73003-c3e5-451b-8b23-89e3fbfad41f)
  - ![Screenshot 2024-08-05 170602](https://github.com/user-attachments/assets/98d54f6c-a4de-4cc3-918b-fae4a55aef3f)
  - ![Screenshot 2024-08-05 161726](https://github.com/user-attachments/assets/c6492619-7ca1-49d4-8998-56b9da849928)


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
