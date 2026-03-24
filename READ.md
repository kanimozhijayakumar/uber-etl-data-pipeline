# 🚖 Uber Data Analytics | End-to-End Data Engineering Project

---

## 📌 Project Overview

This project demonstrates a complete **end-to-end data engineering pipeline** using Uber (NYC Taxi) trip data. The pipeline extracts raw data, transforms it using Python, and loads it into a cloud data warehouse to generate insights.

This project simulates a real-world workflow including:

- Data Ingestion
- ETL Pipeline (Extract, Transform, Load)
- Data Modeling
- Data Warehousing
- Data Visualization

---

## 🏗️ Architecture

![Architecture](architecture.jpg)

### 🔄 Data Flow

1. Ingest raw CSV dataset  
2. Transform data using Python  
3. Store data in Google Cloud Storage  
4. Orchestrate pipeline using Mage  
5. Load data into BigQuery  
6. Build dashboard in Looker Studio  

---

## 🛠️ Tech Stack

### 👨‍💻 Programming
- Python (Pandas, NumPy)

### ☁️ Cloud Platform (GCP)
- Google Cloud Storage
- Compute Engine
- BigQuery
- Looker Studio

### 🔄 Data Pipeline Tool
- Mage AI

---

## 📊 Dataset

- Source: NYC TLC Trip Record Data  
- Contains:
  - Pickup & Drop-off time
  - Location IDs
  - Trip distance
  - Fare amount
  - Payment type
  - Passenger count  

📁 Dataset:  
https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project/blob/main/data/uber_data.csv  

📚 References:
- https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page  
- https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf  

---

## 🧱 Data Model

<p align="center">
  <img src="images/data_model.jpeg" width="800"/>
</p>

### ⭐ Schema Design

- Fact Table: Trip Data  
- Dimension Tables:
  - Date
  - Passenger Count
  - Payment Type
  - Location  

---

## ⚙️ Installation

Run the following commands:

```bash
sudo apt-get update
sudo apt-get install python3-distutils python3-apt wget

wget https://bootstrap.pypa.io/get-pip.py
sudo python3 get-pip.py

pip3 install mage-ai pandas google-cloud google-cloud-bigquery
```

📄 Full commands:  
👉 [Installation Guide](comment.txt)

---

## ⚙️ ETL Pipeline

### 🔹 Extract
- Load raw CSV dataset

### 🔹 Transform
- Remove duplicates
- Handle missing values
- Create Trip ID
- Format datetime columns
- Build dimension tables

### 🔹 Load
- Upload to GCP Storage
- Load into BigQuery

---

## 📈 SQL Analytics

Example insights:

- Total trips per day  
- Revenue analysis  
- Payment type distribution  
- Peak hour demand  

📄 SQL File:
```
sql/analytics_query.sql
```

---

## 📊 Dashboard

- Built using Looker Studio  
- Visualizations include:
  - Revenue trends
  - Trip trends
  - Peak hours
  - Payment distribution  

---

## 📂 Project Structure

```
uber-data-engineering-project/
│
├── data/
│   └── uber_data.csv
│
├── images/
│   ├── architecture.jpg
│   └── data_model.jpeg
│
├── notebooks/
│   └── Uber Data Pipeline.ipynb
│
├── sql/
│   └── analytics_query.sql
│
├── mage-files/
├── comment.txt
├── README.md
```

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/uber-data-engineering-project.git
cd uber-data-engineering-project
pip install pandas numpy jupyter
jupyter notebook
```

---

## 🚀 Key Features

✔ End-to-End Data Pipeline  
✔ Cloud Data Engineering (GCP)  
✔ Real-world Dataset  
✔ Data Modeling (Star Schema)  
✔ ETL Pipeline using Python  
✔ Dashboard Visualization  

