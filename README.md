# Amazon Data Analysis with Databricks & Snowflake

## Overview
This project demonstrates an end-to-end data engineering pipeline for analyzing Amazon product sales data using AWS S3, Databricks, PySpark, and Snowflake. The goal is to ingest, process, transform, and analyze data efficiently, leveraging cloud-based tools and big data technologies.

## Tech Stack
- **AWS S3**: Storage for raw and processed data
- **Databricks**: Data processing and transformation using Apache Spark
- **PySpark**: Distributed data processing framework
- **Snowflake**: Cloud-based data warehouse for analytics
- **Kaggle**: Data source for Amazon product sales data

## Project Structure
```
Amazon-data-analysis-with-Databricks-Snowflake/
│── data/                # Raw dataset stored locally before uploading to S3
│── notebooks/           # Jupyter notebooks for ETL and analysis
│── README.md            # Project documentation
```

## Data Source
- **Amazon Products Sales Dataset 2023**
- Source: [Kaggle](https://www.kaggle.com/datasets/lokeshparab/amazon-products-dataset)

## Workflow

### 1. Data Ingestion
- Create an **AWS S3 bucket** and upload the raw dataset.
- Use the AWS CLI or S3 web console to manage file storage.

### 2. Setting Up Databricks
- Create a **Databricks workspace** and launch a cluster.
- Configure access to S3 using AWS credentials.

### 3. Data Processing with PySpark
- Load the dataset from S3 into a **Databricks notebook**.
- Perform **data cleaning**, **preprocessing**, and **exploratory data analysis (EDA)** using PySpark.

### 4. Data Transformation
- Apply **Spark transformations** to clean and enrich the dataset.
- Convert data into optimized formats (e.g., Parquet, Delta).
- Save processed data back to **S3** for further use.

### 5. Loading Data into Snowflake
- Connect Databricks with **Snowflake**.
- Load the transformed data into Snowflake tables.
- Perform **SQL queries** to generate insights and reports.

## Key Features
✔️ Scalable data processing with **Apache Spark**  
✔️ Cloud storage integration with **AWS S3**  
✔️ Data warehousing with **Snowflake**  
✔️ **ETL pipeline** for structured data transformation  
✔️ **Interactive analysis** using Databricks notebooks  

## Deployment Instructions
### AWS S3 Bucket Setup
To make a file in an **AWS S3 bucket public**:
1. Go to the **AWS S3 Console**.
2. Select the **S3 bucket** containing your file.
3. Click on the file and go to the **Permissions** tab.
4. Click "Edit" under **Public access** settings.
5. Enable "Public access to this object" and save changes.
6. Click **Actions → Make Public** to finalize the process.
7. Copy the public **S3 URL** to share the file.

**⚠️ Security Tip**: Avoid exposing sensitive data publicly. Use IAM roles and bucket policies for controlled access.

## Future Improvements
- Automate ETL pipeline using **Apache Airflow**
- Implement **data validation** and **monitoring**
- Optimize queries in Snowflake for performance
- Visualize insights using **Power BI or Tableau**

## Contributing
Contributions are welcome! Feel free to submit pull requests or open issues for discussions.

## License
This project is licensed under the **MIT License**.

---
🚀 **By Leonel Valencia** | Data Engineering | 2024