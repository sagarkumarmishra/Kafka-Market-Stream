# Kafka-Market-Stream
Real-time stock market data pipeline built using Apache Kafka, AWS (S3, Glue, Athena), and Python. Demonstrated scalable ingestion, transformation, and querying using a modern data lake architecture.
<img width="960" height="540" alt="image" src="https://github.com/user-attachments/assets/c2ba28e6-e7bd-4f76-b7f0-e72fe4e10f60" />


---

## 🗂️ Dataset

- Dataset Name: `indexProcessed.csv`
- Source: 
- Description: Simulated real-time stock ticker data

---

## 🚀 Features

✅ Real-time ingestion with Kafka  
✅ Data lake storage in S3  
✅ Automated metadata generation via AWS Glue  
✅ SQL querying using Amazon Athena  
✅ Deployed Kafka Broker on AWS EC2

---

## 🔍 Sample Athena Query

```sql
SELECT symbol, MAX(price) AS highest_price
FROM "stock_database"."stock_table"
GROUP BY symbol
ORDER BY highest_price DESC
LIMIT 10;

