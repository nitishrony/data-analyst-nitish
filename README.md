# AWS Data Analytic Platform for The City of Vancouver - Part 2

## Project Overview
This project enhances data security, governance, and monitoring for the AWS-based Data Analytic Platform designed for the City of Vancouver. The key focus areas included implementing data protection using AWS KMS, establishing data governance practices through AWS Glue, and setting up data monitoring using AWS CloudWatch.

## Objective
To secure data, automate data governance, and monitor platform performance effectively to ensure data integrity, operational efficiency, and cost management.

## Methodology

### 1. Data Protection
- **KMS Key Creation:**  
  Created AWS KMS keys to encrypt data in S3 buckets, ensuring authorized access only.
- **Bucket Encryption and Replication:**  
  Applied KMS keys to S3 buckets with encryption properties. Backup buckets were set up using S3 replication rules with versioning to protect against data loss.

### 2. Data Governance
- **Trusted Folders and Quality Pipelines:**  
  Created 'Trusted' folders in S3 for quality-checked data. Used AWS Glue to set up ETL pipelines for filtering records based on data quality.
- **Workflow Automation:**  
  Implemented AWS Glue workflows to automate data governance processes, scheduled to run weekly to maintain consistent data quality checks.

### 3. Data Monitoring
- **AWS CloudWatch Dashboards:**  
  Configured dashboards in CloudWatch to track key metrics like billing and S3 usage. Set up alerts for cost thresholds.
- **CloudTrail Monitoring:**  
  Enabled AWS CloudTrail for logging and monitoring API calls, aiding in auditing and security management.

### 4. Architecture Analysis and Optimization
- **Operational Excellence:**  
  Utilized AWS CloudWatch for proactive monitoring and automation, enhancing operational workflows.
- **Security and Reliability:**  
  Ensured data security with AWS KMS and improved reliability through S3 replication and versioning.
- **Cost Optimization and Sustainability:**  
  Monitored costs using AWS Cost Explorer and optimized storage with S3 Intelligent-Tiering to align with sustainability goals.

## Tools and Technologies
- **AWS S3:** For secure data storage with encryption and replication.
- **AWS Glue:** For ETL processes, data quality checks, and workflow automation.
- **AWS KMS:** For encryption key management and data protection.
- **AWS CloudWatch:** For resource monitoring and alert configuration.
- **AWS CloudTrail:** For auditing API calls and tracking changes.

## Deliverables
- Encrypted and backed-up datasets in S3 with versioning.
- Trusted data storage with validated data quality.
- Automated workflows for continuous data governance.
- Real-time monitoring dashboards in CloudWatch.
- Detailed audit logs through CloudTrail.

## Conclusion
This phase of the project successfully integrated AWS services to secure, govern, and monitor the data analytic platform for the City of Vancouver. The implemented solutions provided robust data protection, automated governance processes, and comprehensive monitoring capabilities, ensuring the platform's security, efficiency, and cost-effectiveness.

## Author
- **Nitish Rony**  
- **Team Members:** Amit Rathore, Midhuna Sijoy, Sankeerthana Saini

