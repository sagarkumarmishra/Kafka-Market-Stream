# Kafka-Market-Stream
Real-time stock market data pipeline built using Apache Kafka, AWS (S3, Glue, Athena), and Python. Demonstrated scalable ingestion, transformation, and querying using a modern data lake architecture.

<img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/c2ba28e6-e7bd-4f76-b7f0-e72fe4e10f60" />




## 🔧 Tech Stack

- **Programming**: Python  
- **Streaming**: Apache Kafka  
- **Cloud**: AWS (S3, EC2, Glue, Athena)  
- **Data Lake Storage**: Amazon S3  
- **Metadata & ETL**: AWS Glue Crawler & Catalog  
- **SQL Analytics**: Amazon Athena



## 🗂️ Dataset

- **File**: `indexProcessed.csv`  
- **Source**: https://github.com/sagarkumarmishra/Kafka-Market-Stream/blob/main/indexProcessed.csv
- **Description**: Simulated stock ticker data for real-time ingestion



## 🚀 Features

- ✅ Real-time stock data ingestion using Kafka
- ✅ Cloud-based storage using Amazon S3
- ✅ Schema inference using AWS Glue Crawler
- ✅ SQL-based analytics using Athena
- ✅ Kafka deployed on EC2 instance



## 🔍 Sample Athena Query

```sql
SELECT symbol, MAX(price) AS highest_price
FROM "stock_database"."stock_table"
GROUP BY symbol
ORDER BY highest_price DESC
LIMIT 10;

# 🎯 Learning Outcomes

- Understand Kafka’s producer-consumer mechanism  
- Deploy Kafka on AWS EC2  
- Ingest and store real-time data in S3  
- Create Glue Crawlers and Catalogs  
- Query datasets using Amazon Athena (SQL)  
