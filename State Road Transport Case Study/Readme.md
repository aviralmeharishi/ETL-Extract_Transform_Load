# 🚛 ETL Pipeline Case Study – State Road Transport Data

[![ETL](https://img.shields.io/badge/Project-ETL%20Pipeline-blue)](#)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen)](#)
[![Python](https://img.shields.io/badge/Python-Notebook-yellowgreen)](#)

> A case study on building a complete **ETL pipeline** using multi-format government transport datasets with cloud storage integration and Tableau visualization.

---

## 📁 Data Sources

The data was sourced from the [Government of India Open Data Portal](https://data.gov.in/) and includes:

- 📄 **CSV**: Profit and Loss data  
- 🧾 **JSON**: Financial performance data  
- 🗂 **XML**: Physical data of SRTUs  

All datasets are hypothetically stored in **Google Drive** (cloud storage).

---

## 🔁 ETL Process Overview

```mermaid
graph TD
    A[📥 Extract] --> B[🛠 Transform]
    B --> C[📤 Load]
    

