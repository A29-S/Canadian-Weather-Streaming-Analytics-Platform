<h1 align="center">
🌦️ Canadian Weather Data Engineering & Analytics Pipeline
</h1>

<p align="center">
End-to-End Data Engineering • Streaming Pipelines • Machine Learning • Interactive Analytics
</p>

<p align="center">
<img src="https://img.shields.io/badge/Python-3.9+-blue">
<img src="https://img.shields.io/badge/Apache-Kafka-black">
<img src="https://img.shields.io/badge/Apache-Spark-orange">
<img src="https://img.shields.io/badge/Streamlit-Dashboard-red">
<img src="https://img.shields.io/badge/Database-SQLite-lightgrey">
<img src="https://img.shields.io/badge/ML-ScikitLearn-green">
</p>

---

# 🚀 Live Demo

### Interactive Streamlit Dashboard

🔗 **Launch the Dashboard**

https://weather-dashboard-group6.streamlit.app

---

# 📊 Project Overview

This project builds an **end-to-end data engineering and analytics pipeline** for exploring Canadian climate data.

The system processes historical weather datasets and simulates a **real-time streaming architecture** where weather observations are ingested, processed, and analyzed through an interactive dashboard.

The platform allows users to:

✔ Explore **long-term weather trends**  
✔ Detect **extreme weather events**  
✔ Perform **statistical analysis**  
✔ Run **regression models on climate variables**  
✔ Visualize **interactive time-series data**

---

# 🧠 Skills Demonstrated

This project highlights experience in:

- Data Engineering  
- Streaming Data Pipelines  
- Big Data Processing  
- Machine Learning  
- Interactive Data Visualization  

---

# 🏗️ System Architecture

The platform simulates a **real-time streaming pipeline for climate analytics**.
Government Climate Data (CSV)
│
▼
Data Cleaning & Transformation
(Python / Pandas)
│
▼
Kafka Producer
│
▼
Spark Streaming
│
▼
SQLite Analytics Database
│
▼
Streamlit Dashboard
│
▼
Statistical Analysis & ML Models

Government Climate Data (CSV)
│
▼
Data Cleaning & Transformation
(Python / Pandas)
│
▼
Kafka Producer
│
▼
Spark Streaming
│
▼
SQLite Analytics Database
│
▼
Streamlit Dashboard
│
▼
Statistical Analysis & ML Models


---

# ⚙️ Technologies Used

| Category | Tools |
|--------|--------|
| Programming | Python |
| Streaming | Apache Kafka |
| Big Data Processing | Apache Spark Streaming |
| Data Processing | Pandas |
| Machine Learning | Scikit-Learn |
| Visualization | Streamlit |
| Database | SQLite |

---

# 🌎 Dataset

The data is sourced from the **Government of Canada Climate Data Portal**.

### Climate Variables

- Temperature *(minimum / maximum / median)*
- Precipitation *(rain / snow)*
- Wind speed
- Atmospheric pressure
- Weather station metadata

### Locations Analyzed

🇨🇦 Toronto  
🇨🇦 Vancouver  
🇨🇦 Edmonton  
🇨🇦 Halifax  
🇨🇦 St George  
🇨🇦 Inuvik  

---

# 🔧 Key Features

---

## 📦 Data Pipeline

The pipeline processes raw weather station datasets and converts them into **structured analytical datasets**.

### Processing Steps

- Parsing temporal fields into **datetime objects**
- Feature extraction *(year, month, season)*
- Handling **missing values**
- Standardizing **weather measurements**
- Aggregating **station-level observations**

---

## 🔄 Streaming Architecture

Kafka acts as a **message broker** that streams weather observations into the analytics pipeline.

Spark Streaming processes incoming records and writes them to a **structured SQLite analytics database**.

This architecture simulates a **real-time ingestion pipeline** that could easily be extended to **live climate data feeds**.

---

## Streaming Pipeline Diagram

<p align="center">
<img src="https://github.com/user-attachments/assets/66c0b418-6871-4b7b-b699-a87b4a650449" width="900">
</p>

---

## 📊 Interactive Dashboard

The **Streamlit dashboard** allows users to explore the dataset through multiple analytical tools.

### Users Can

✔ Filter by **location**  
✔ Select **climate variables**  
✔ Explore **seasonal trends**  
✔ Visualize **time-series data**  
✔ Generate **descriptive statistics**

---

## 🌡️ Extreme Event Detection

The dashboard includes tools to identify **extreme climate events**.

Users can define thresholds to detect:

🔥 Heat waves  
🌧 Heavy precipitation  
💨 High wind events  

This enables exploration of **climate anomalies across regions**.

---

## 📈 Statistical Analysis

The dashboard supports several statistical tools.

---

## Descriptive Statistics

Provides key dataset summaries:

- Mean
- Standard deviation
- Quartiles

---

## Correlation Analysis

A **correlation matrix** visualizes relationships between climate variables such as:

- Temperature
- Precipitation
- Wind speed
- Atmospheric pressure

---

## Regression Modeling

### Simple Linear Regression

Predicts one variable from another.

Example:

Temperature vs Atmospheric Pressure

---

### Multiple Linear Regression

Predicts weather outcomes using multiple predictors.

Model outputs include:

- Regression coefficients
- **R² score**
- Predicted vs actual plots
- Residual plots

---

# 🖥️ Example Dashboard Outputs

---

## Dashboard Overview

<p align="center">
<img src="https://github.com/user-attachments/assets/a21e8a6e-2259-418a-8969-3167f368a22b" width="900">
</p>

---

## Extreme Events  
**Summer Months in Toronto above 22°C (1840–1999)**

<p align="center">
<img src="https://github.com/user-attachments/assets/5553934a-1fa4-4f09-85af-4c6b2189c0e3" width="900">
</p>

---

## Time Series Example  
**Mean Precipitation in April (1990–1999)**

<p align="center">
<img src="https://github.com/user-attachments/assets/5d734729-574f-4a96-af82-701a764dfefc" width="900">
</p>

---

## Correlation Matrix

<p align="center">
<img src="https://github.com/user-attachments/assets/03b7356b-5869-4ce0-b748-84ee4d956fc5" width="900">
</p>

---

## Scatterplot Analysis

<p align="center">
<img src="https://github.com/user-attachments/assets/e6d3c7ed-9079-454e-9668-c95b8b183fb1" width="900">
</p>

---

## Multiple Linear Regression Output

<p align="center">
<img src="https://github.com/user-attachments/assets/42a106b9-9ef8-4fc5-8e8e-1fdc705bc3a2" width="900">
</p>

# ▶️ Running the Project

Follow these steps to run the weather streaming pipeline locally.

---

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/weather-streaming-dashboard
cd weather-streaming-dashboard
2️⃣ Install Dependencies

Install all required Python packages.

pip install -r requirements.txt
3️⃣ Start Kafka Producer

This script streams weather observations into the Kafka pipeline.

python kafka_producer.py
4️⃣ Run Spark Streaming Job

The Spark job consumes Kafka messages and writes processed records to the analytics database.

spark-submit streaming_job.py
5️⃣ Launch the Dashboard

Start the interactive analytics dashboard.

streamlit run dashboard.py

The dashboard will open in your browser at:

http://localhost:8501
