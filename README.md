# Data-Analyst-Nitish
# Mountain View Cemetery Burial Index Analysis

## Project Overview
This project involves analyzing the burial patterns in the Mountain View Cemetery from 1893 to 2003. The analysis calculates the percentage of burials per decade, providing insights into historical burial trends over time.

## Objective
The primary objective of this project is to analyze burial data to identify patterns and trends in burials across different decades, helping to understand changes over time.


## Dataset
- **Source:** Mountain View Cemetery Burial Index from the City of Vancouver's open data portal.
- **Content:** Records of burials including burial date, name, and other attributes.
- [mountain-view-cemetery-burial-index.xlsx](https://github.com/user-attachments/files/17036567/mountain-view-cemetery-burial-index.xlsx)


## Methodology
- ![Screenshot 2024-09-17 170223](https://github.com/user-attachments/assets/92f9b220-b5f7-4f2f-8d38-fa5c0aec770f)

1. **Data Collection and Ingestion:**  
   - Data ingested into AWS S3, organized in landing, raw, and curated folders.
   - ![image](https://github.com/user-attachments/assets/a0be5ddb-d1ff-4b72-a6fa-43a14f5f2df8)
   - ![image](https://github.com/user-attachments/assets/daaf9df7-81f5-467b-bb6c-d120753d1704)


   
2. **Data Cleaning:**  
   - Cleaned the dataset to remove missing or invalid values, ensuring data quality.
   - ![image](https://github.com/user-attachments/assets/41129dd8-b281-4159-867b-247f6e2991ec)

   
3. **Data Structuring:**  
   - Reorganized the dataset by renaming columns, adjusting data types, and extracting necessary information (e.g., year from burial dates).
  
   - ![image](https://github.com/user-attachments/assets/27db912b-fe87-4974-9348-866d86d9e7b9)

   
4. **ETL Pipeline Design and Implementation:**  
   - Built an ETL pipeline using AWS Glue for data transformation, including schema changes and calculating burial percentages per decade.
  
   - ![image](https://github.com/user-attachments/assets/ea74dcbc-1deb-467c-a30a-68afc77a622c)

   
5. **Data Analysis:**  
   - Used AWS Athena to run SQL queries on the curated dataset to calculate decade-wise burial percentages.
  
   - ![image](https://github.com/user-attachments/assets/df8aa745-c80b-4c45-9bba-915c6b3f5685)
   - ![image](https://github.com/user-attachments/assets/3213b71b-7fca-4d47-925b-71e738d776e4)

   
6. **Data Visualization:**  
   - Visualized the burial trends using Excel due to limitations with AWS QuickSight access.
   - ![image](https://github.com/user-attachments/assets/fb3b71e6-92b9-431a-b851-59931bdd8e84)

   
7. **Data Publishing:**  
   - Published results on AWS EC2 servers for internal and public access.
   - ![image](https://github.com/user-attachments/assets/01731bc4-b203-4ea2-874b-2cef89e78194)


## Tools and Technologies
- **AWS S3:** Data storage and management.
- **AWS Glue:** ETL pipeline for data processing.
- **AWS Athena:** Data querying and analysis.
- **Excel:** Data visualization.
- **AWS EC2:** Hosting and publishing results.

## Deliverables
- Cleaned and structured dataset from Mountain View Cemetery (1893-2003).
- Graphs depicting burial trends per decade.
- Detailed report documenting the ETL process, data analysis, and key findings.
- Published results accessible through EC2 servers.

## Conclusion
This project provided valuable insights into historical burial patterns at Mountain View Cemetery, which can aid in historical research and cemetery management.

## Author
- **Nitish Rony**
