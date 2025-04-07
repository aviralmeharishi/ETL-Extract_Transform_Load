# 🧠 Depression Detection with SQL + Python 🔍

> **Can we decode the signs of depression with just data? Let’s find out.**

Welcome to my mental health mini-project where I blend **SQL, Python, and Data Analysis** to explore indicators of depression. It’s a step toward turning raw data into actionable insights—and maybe even saving lives ❤️.

---

## 📊 Dataset in a Nutshell

- **Name**: `Depressed!!!.xlsx`
- **Size**: **15,000 rows × 23 columns**
- **Contents**: A mix of **demographics**, **lifestyle habits**, and **psychological factors** to analyze depression trends.
- **Stored In**: MySQL database (`depression_db`)
- **Table Name**: `depression_data`

---

## 🔗 Tech Stack

| Tool         | Purpose                         |
|--------------|----------------------------------|
| Python 🐍     | Scripting, Data Analysis         |
| MySQL 🛢️      | Data Storage & Querying          |
| Pandas 🐼     | Data Manipulation                |
| SQLAlchemy ⚙️| Python-DB Bridge                 |
| Jupyter 📓    | Interactive Exploration          |

---

## ⚙️ Project Flow

### ✅ 1. Data Upload & Storage

- Read the Excel file using `pandas.read_excel()`
- Clean the data (nulls, renaming, formatting)
- Push it to MySQL using `pymysql` or `sqlalchemy`

### ✅ 2. Querying with SQL in Python

Here’s a sneak peek of how I’m running queries right from Python:

```python
from sqlalchemy import create_engine
import pandas as pd

engine = create_engine("mysql+pymysql://username:password@localhost/depression_db")
query = "SELECT Gender, COUNT(*) AS Count FROM depression_data GROUP BY Gender"
df = pd.read_sql(query, engine)
print(df)

