# AWS Data Analytic Platform for The City of Vancouver - Part 2

## Project Overview
This project enhances data security, governance, and monitoring for the AWS-based Data Analytic Platform designed for the City of Vancouver. The key focus areas included implementing data protection using AWS KMS, establishing data governance practices through AWS Glue, and setting up data monitoring using AWS CloudWatch.

## Objective
To secure data, automate data governance, and monitor platform performance effectively to ensure data integrity, operational efficiency, and cost management.

## Methodology
![image](https://github.com/user-attachments/assets/8a654513-2e7d-408c-bb8a-84b613a67b4b)


### 1. Data Protection
- **KMS Key Creation:**  
  Created AWS KMS keys to encrypt data in S3 buckets, ensuring authorized access only.
  ![image](https://github.com/user-attachments/assets/2c29defc-4c10-4577-9820-d5abfb6e0070)

- **Bucket Encryption and Replication:**  
  Applied KMS keys to S3 buckets with encryption properties. Backup buckets were set up using S3 replication rules with versioning to protect against data loss.
  ![image](https://github.com/user-attachments/assets/25d0af99-a2ce-440a-a9cf-a3d673c1e71d)
  ![image](https://github.com/user-attachments/assets/ae4e746f-e650-40d6-998a-af4c4bbf683f)
  ![image](https://github.com/user-attachments/assets/ae8eb2b1-ba2f-4e58-add5-fa988666e719)




### 2. Data Governance
- **Trusted Folders and Quality Pipelines:**  
  Created 'Trusted' folders in S3 for quality-checked data. Used AWS Glue to set up ETL pipelines for filtering records based on data quality.
  ![image](https://github.com/user-attachments/assets/e0615513-f666-42f9-947f-a75ca3b6114a)
  ![image](https://github.com/user-attachments/assets/9556230f-d0bf-40b3-9d15-16cd3ece2d02)
  ![image](https://github.com/user-attachments/assets/8dfb9ed0-aa68-4889-943c-482649dc2bfc)


- **Workflow Automation:**  
  Implemented AWS Glue workflows to automate data governance processes, scheduled to run weekly to maintain consistent data quality checks.
  ![image](https://github.com/user-attachments/assets/b6a9e4f1-7da4-49c9-99c7-4b6a37483dc8)
  ![image](https://github.com/user-attachments/assets/21916e16-83a2-435e-be2b-57fa40c351ad)



### 3. Data Monitoring
- **AWS CloudWatch Dashboards:**  
  Configured dashboards in CloudWatch to track key metrics like billing and S3 usage. Set up alerts for cost thresholds.
  ![image](https://github.com/user-attachments/assets/e363b1c5-efa3-4889-b2eb-e3cea46f6806)
  ![image](https://github.com/user-attachments/assets/90401ef7-6287-4fce-9a23-dba32d2eb983)


- **CloudTrail Monitoring:**  
  Enabled AWS CloudTrail for logging and monitoring API calls, aiding in auditing and security management.
  ![image](https://github.com/user-attachments/assets/917e066b-2ed2-4bd1-91e9-95dbf37707af)
  ![image](https://github.com/user-attachments/assets/e1430082-56de-4f1b-9e9c-cb93b33ee0b5)


### 4. Architecture Analysis and Optimization
- **Operational Excellence:**  
  Utilized AWS CloudWatch for proactive monitoring and automation, enhancing operational workflows.
- **Security and Reliability:**  
  Ensured data security with AWS KMS and improved reliability through S3 replication and versioning.


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

