## 🧾 Data Description

The project utilizes publicly available datasets from **State Road Transport Undertakings (SRTUs)** in India, sourced from [data.gov.in](https://data.gov.in/). These datasets are provided in **multiple formats** representing different types of information:

### 📂 File Types & Contents

| Format | File Type | Description |
|--------|-----------|-------------|
| 📄 CSV   | Structured   | Profit & Loss data for SRTUs |
| 🧾 JSON  | Semi-Structured | Financial performance data (e.g., income, expenses) |
| 🗂 XML   | Semi-Structured | Physical data (e.g., number of buses, kilometers operated) |

### 🧠 Key Attributes Across Datasets

- `State_Name`: Name of the state
- `Year`: Reporting year
- `Total_Revenue`: Total income/revenue (from JSON)
- `Operating_Expenses`: Costs incurred (from JSON)
- `Net_Profit_Loss`: Profit or loss (from CSV)
- `No_of_Buses`: Physical asset count (from XML)
- `Distance_Covered`: Kilometers run (from XML)

> 💡 **Note:** Column names were cleaned and standardized during transformation to ensure consistency across all formats.

---

### 🗃 Sample Rows (After Transformation)

| State     | Year | Revenue | Expenses | Profit/Loss | Buses | KM Run |
|-----------|------|---------|----------|-------------|--------|--------|
| Gujarat   | 2020 | 100 Cr  | 95 Cr    | 5 Cr        | 1200   | 3.5M   |
| Maharashtra | 2020 | 220 Cr | 230 Cr   | -10 Cr      | 2100   | 6.7M   |

---

📌 The cleaned, merged dataset is stored in `final_data.xlsx` and used for further visualization in Tableau.
