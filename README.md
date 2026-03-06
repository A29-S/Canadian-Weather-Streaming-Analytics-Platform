Project Overview

This project builds an end-to-end data engineering and analytics pipeline for exploring Canadian weather data.

The system processes historical climate data and simulates a real-time streaming architecture where weather observations are ingested, processed, and analyzed through an interactive dashboard.

The platform allows users to:

Explore long-term weather trends

Detect extreme weather events

Perform statistical analysis

Run regression models on climate variables

The project demonstrates skills in:

Data Engineering

Streaming Data Pipelines

Machine Learning

Interactive Data Visualization

Big Data Processing

Live Demo

Streamlit Dashboard
(weather-dashboard-group6.streamlit.app)

Architecture

Data flows through a streaming pipeline:

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

Technologies used:

Python

Apache Kafka

Apache Spark Streaming

SQLite

Pandas

Scikit-Learn

Streamlit

Dataset

Data comes from the Government of Canada Climate Data Portal.

Variables include:

Temperature (min / max / median)

Precipitation (rain / snow)

Wind speed

Atmospheric pressure

Geographic station metadata

Locations analyzed:

Toronto

Vancouver

Edmonton

Halifax

St George

Inuvik

Key Features
Data Pipeline

The pipeline processes raw weather station datasets and transforms them into structured analytical datasets.

Steps include:

Parsing temporal fields into datetime objects

Feature extraction (year, month, season)

Handling missing values

Standardizing weather measurements

Aggregating station-level observations

Streaming Architecture

Data processing pipeline
<img width="1412" height="820" alt="image" src="https://github.com/user-attachments/assets/66c0b418-6871-4b7b-b699-a87b4a650449" />


Kafka acts as a message broker that streams weather observations into the analytics pipeline.

Spark Streaming processes the incoming records and writes them to a structured SQLite analytics database.

This architecture simulates a real-time data ingestion pipeline that could be extended to live climate data feeds.

Interactive Dashboard

The Streamlit dashboard allows users to explore the dataset through multiple analytical tools.

Users can:

Filter by location

Select variables

Explore seasonal trends

Visualize time series data

Generate descriptive statistics

Extreme Event Detection

The dashboard includes tools to detect extreme weather events.

Users can define thresholds to identify:

Heat waves

Heavy precipitation

High wind events

This enables exploration of climate anomalies across regions.

Statistical Analysis

The dashboard supports several statistical tools:

Descriptive Statistics

Summary statistics including:

Mean

Standard deviation

Quartiles

Correlation Analysis

A correlation matrix visualizes relationships between climate variables such as:

Temperature

Precipitation

Wind speed

Atmospheric pressure

Regression Modeling

The system supports:

Simple Linear Regression

Predicting one variable from another.

Example:

Temperature vs Atmospheric Pressure

Multiple Linear Regression

Predicting weather outcomes using multiple predictors.

Outputs include:

Regression coefficients

R² score

Predicted vs actual plots

Residual plots

Example Dashboard Output
Dashboard Overview
<img width="2241" height="1388" alt="image" src="https://github.com/user-attachments/assets/a21e8a6e-2259-418a-8969-3167f368a22b" />

Extreme Events: Summer Months in Toronto above 22C from 1840 - 1999
<img width="2237" height="1384" alt="image" src="https://github.com/user-attachments/assets/5553934a-1fa4-4f09-85af-4c6b2189c0e3" />

Time Series for Mean Precipitation in April from 1990 - 1999
<img width="2232" height="1383" alt="image" src="https://github.com/user-attachments/assets/5d734729-574f-4a96-af82-701a764dfefc" />

Correlation Matrix
<img width="2243" height="1398" alt="image" src="https://github.com/user-attachments/assets/03b7356b-5869-4ce0-b748-84ee4d956fc5" />

Scatterplot
<img width="2255" height="1106" alt="image" src="https://github.com/user-attachments/assets/e6d3c7ed-9079-454e-9668-c95b8b183fb1" />

MLR
<img width="2280" height="1341" alt="image" src="https://github.com/user-attachments/assets/42a106b9-9ef8-4fc5-8e8e-1fdc705bc3a2" />


