# 📈 Financial Market Data ETL Pipeline

This project implements a robust and scalable ETL pipeline that extracts real-time and historical financial market data from **Alpha Vantage** and **Yahoo Finance**, transforms the data using **PySpark**, orchestrates the workflow with **Apache Airflow**, and loads the processed data into a **PostgreSQL** database for analysis and reporting.

---

## 📚 Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Pipeline Architecture](#pipeline-architecture)
- [Features](#features)
- [Getting Started](#getting-started)
- [Environment Variables](#environment-variables)
- [Project Structure](#project-structure)
- [License](#license)

---

## 🧠 Overview

The goal of this pipeline is to automate the extraction, transformation, and loading of stock market data from public APIs into a centralized data warehouse for financial analytics, dashboards, and forecasting models.

---

## 🧰 Tech Stack

- 🐍 **Python** – scripting and automation  
- ⚙️ **Apache Airflow** – pipeline orchestration  
- 🔥 **PySpark** – data transformation at scale  
- 🐘 **PostgreSQL** – storage for transformed data  
- 🌐 **Alpha Vantage & Yahoo Finance APIs** – data sources  

---

## 🔄 Pipeline Architecture

```text
        +---------------------+
        |   Alpha Vantage     |
        |   Yahoo Finance     |
        +----------+----------+
                   |
                   v
          [Data Extraction Layer]
                   |
                   v
         [Raw Data Landing Zone]
                   |
                   v
           [PySpark Transformations]

                   |
                   v
        [Transformed Data Warehouse]
                   |
                   v
         [PostgreSQL for Analysis]
---

## ✨ Features

- ✅ **Scheduled and automated data pulls** from Alpha Vantage and Yahoo Finance  
- ⚡ **Scalable data transformation using PySpark** (e.g., cleaning, deduplication, formatting)  
- 🔄 **Workflow orchestration and monitoring with Airflow DAGs**  
- 🔐 **Secure environment variable handling**  
- 🐘 **PostgreSQL integration** for data storage and downstream analytics  
