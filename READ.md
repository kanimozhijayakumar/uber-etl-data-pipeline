# 🚖 Uber Data Analytics | End-to-End Data Engineering Project

---

## 📌 Project Overview

This project demonstrates a complete **end-to-end data engineering pipeline** using Uber (NYC Taxi) trip data. The pipeline extracts raw data, transforms it using Python, loads it into a cloud data warehouse, and generates insights through dashboards.

This project simulates a real-world data engineering workflow including:

- Data Ingestion
- Data Transformation (ETL)
- Data Modeling
- Data Warehousing
- Data Visualization

---

## 🏗️ Architecture

![Architecture](architecture.jpg)

### 🔄 Data Flow

1. Raw data ingestion from CSV dataset
2. Data cleaning and transformation using Python
3. Upload to Google Cloud Storage (Data Lake)
4. Pipeline orchestration using Mage
5. Load transformed data into BigQuery
6. Build dashboard using Looker Studio

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
- Mage AI (https://www.mage.ai/)

---

## 📊 Dataset

- **Source:** NYC TLC Trip Record Data
- Includes:
  - Pickup & Drop-off timestamps
  - Location IDs
  - Trip distance
  - Fare amount
  - Payment type
  - Passenger count

📁 Dataset used:  
https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project/blob/main/data/uber_data.csv

📚 References:
- https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
- https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

---

## 🧱 Data Modeling

![Data Model](data_model.jpeg)

### ⭐ Schema Design (Star Schema)

- **Fact Table:**
  - Trip Data

- **Dimension Tables:**
  - Date Dimension
  - Passenger Count
  - Payment Type
  - Pickup & Drop Location

---

## ⚙️ ETL Pipeline

### 🔹 Extract
- Load raw CSV dataset

### 🔹 Transform
- Handle missing values
- Remove duplicates
- Create unique Trip ID
- Format datetime columns
- Build dimension tables

### 🔹 Load
- Upload data to GCP Storage
- Load into BigQuery tables

---

## 📈 SQL Analytics

Example insights:

- Total trips by date
- Revenue analysis
- Payment type distribution
- Peak hour demand

📄 SQL file:
```
sql/analytics_query.sql
```

---

## 📊 Dashboard

- Built using Looker Studio
- Interactive visualizations:
  - Trip trends
  - Revenue trends
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
├── notebooks/
│   └── Uber Data Pipeline.ipynb
│
├── sql/
│   └── analytics_query.sql
│
├── mage-files/
│
├── architecture.jpg
├── data_model.jpeg
├── README.md
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone Repository

```bash
git clone https://github.com/kanimozhiyjayakumar/uber-data-engineering-project.git
cd uber-data-engineering-project
```

### 2️⃣ Install Dependencies

```bash
pip install pandas numpy jupyter
```

### 3️⃣ Run Notebook

```bash
jupyter notebook
```

### 4️⃣ Execute ETL Pipeline

- Run all cells in notebook
- Upload output to GCP
- Load into BigQuery

---

## 🚀 Key Features

✔ End-to-End Data Pipeline  
✔ Cloud Integration (GCP)  
✔ Real-world Dataset  
✔ Data Modeling (Star Schema)  
✔ ETL Pipeline using Python  
✔ Dashboard Visualization  

---

## 📌 Future Improvements

- Add Apache Airflow orchestration  
- Dockerize the pipeline  
- Real-time streaming using Kafka  
- CI/CD integration  
- Data quality validation  

---

## 🤝 Contribution

Contributions are welcome!  
Feel free to fork and improve this project.

---

