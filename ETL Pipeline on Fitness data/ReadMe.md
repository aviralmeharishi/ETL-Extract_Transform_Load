# 🧠 ETL Pipeline on Fitness & Obesity Data

This project showcases a complete **ETL (Extract, Transform, Load) pipeline** applied to real-world fitness and obesity-related lifestyle data. The goal was to clean, simplify, and standardize the dataset, and store it in a relational database for downstream machine learning and analytics tasks.

---

## 🚀 Project Workflow

- 🔍 **Extract**: Load raw data from a `.csv` file.
- 🔧 **Transform**:
  - Clean and rename columns for readability
  - Merge inconsistent categorical values (e.g., `no` and `nope`)
  - Simplify complex target labels into user-friendly classes
  - Apply SQL-based column updates and restructuring
- 💾 **Load**: Store the final cleaned dataset in a MySQL table.

---

## 🔁 Schema: Before vs After

| **Old Column Name**  | **New Column Name**        | **Description**                                                   |
|----------------------|----------------------------|-------------------------------------------------------------------|
| `FAVC`               | `high_calorie_food_intake` | High-calorie food consumption (Yes/No)                            |
| `FCVC`               | `veggie_frequency`         | Frequency of vegetable consumption (Scale: 1 to 3)                |
| `NCP`                | `no_of_meals`              | Number of main meals per day                                     |
| `CAEC`               | `snacking_freq`            | Snacking between meals (Never/Sometimes/Frequently/Always)       |
| `SMOKE`              | `smoking_status`           | Smoking habit (Yes/No)                                           |
| `CH2O`               | `water_consumption`        | Daily water intake (Scale: 1 to 3)                                |
| `SCC`                | `calorie_monitoring`       | Whether calories are monitored (Yes/No)                           |
| `FAF`                | `physical_activity`        | Frequency of physical activity (Scale: 0 to 3)                    |
| `TUE`                | `time_spend_on_tech`       | Time spent on technology daily (Scale: 0 to 3)                    |
| `CALC`               | `alcohol_consump`          | Alcohol consumption frequency                                     |
| `MTRANS`             | `transport_mode`           | Primary mode of transportation                                    |
| `NObeyesdad`         | `health_condition`         | Simplified obesity level: Underweight, Healthy, Overweight, etc. |

---

## 🧠 What Was Improved?

- ✅ Merged inconsistent values (e.g., `'nope'` → `'no'`)
- ✅ Renamed cryptic column names to meaningful labels
- ✅ Simplified 7-class target (`NObeyesdad`) into 5 user-friendly categories:
  - Underweight, Healthy, Overweight, Obese, Severely Obese
- ✅ Applied SQL-based updates and renaming directly to the database
- ✅ Verified schema and imported clean data into Python for further use

---

## 📂 Project Structure

```
├── ETL Pipeline on Fitness Data.ipynb   # Jupyter notebook with full ETL logic
├── obesity_data.csv                     # Raw dataset
├── README.md                            # Project documentation
```

---

## 🛠️ Tools & Technologies

| Purpose        | Tools Used            |
|----------------|------------------------|
| IDE            | VS Code                |
| Data Handling  | Python (Pandas, NumPy) |
| Database       | MySQL                  |
| Notebook       | Jupyter Notebook       |

---

## ✅ Key Outcomes

- Fully working ETL pipeline using SQL + Python
- Database-ready schema for future model training or dashboarding
- Clean, simplified data structure for better interpretability

---

## 💡 Future Enhancements

- Add automated ETL scheduling (e.g., `schedule` or `cron`)
- Train and evaluate a multi-class ML model on the cleaned data
- Build an interactive web app using Streamlit or FastAPI

---

## 🙌 Acknowledgements

- Dataset based on real-life health & fitness factors
- Project built to demonstrate practical ETL and SQL skills in action

---

## 📬 Connect with Me

- 🔗 [LinkedIn](https://www.linkedin.com/in/aviral-meharishi-50879632b/)
- 💻 [GitHub](https://github.com/aviralmeharishi)
- 📧 aviralmeharishi@gmail.com

