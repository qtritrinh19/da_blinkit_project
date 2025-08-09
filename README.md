# Blinkit Retail Sales & Revenue Analysis

## 📌 Project Overview
This project demonstrates a complete data analytics workflow using **Python**, **MS SQL Server**, and **Power BI**.  
The dataset, sourced from [Kaggle - Blinkit Sales Dataset](https://www.kaggle.com/datasets/akxiit/blinkit-sales-dataset/data), is cleaned and prepared in Python, stored in MS SQL Server, and visualized in an interactive Power BI dashboard.

---

## 🎯 Objectives
- Build a reproducible **ETL pipeline** from raw CSV to BI dashboard.
- Practice **data cleaning and preprocessing** using Python.
- Store processed data in **MS SQL Server** to simulate real-world database integration.
- Create an interactive dashboard in **Power BI** for business insights.

---

## 🛠️ Workflow & Methodology

### 1️⃣ Data Acquisition
- Downloaded the Blinkit sales dataset from Kaggle in CSV format.

### 2️⃣ Data Preprocessing in Python
- Libraries used: **Pandas**, **NumPy**.
- Tasks performed:
  - Removed duplicate and invalid entries.
  - Standardized date formats and categorical fields.
- Output: Cleaned dataset stored in a Pandas DataFrame.

### 3️⃣ Database Setup in MS SQL Server
- Established a connection to MS SQL Server using **SQLAlchemy**.
- Created a database table schema to match the cleaned dataset.
- Loaded the DataFrame into SQL Server with `to_sql()` method.

### 4️⃣ Data Visualization in Power BI
- Connected Power BI directly to MS SQL Server.
- Created an interactive dashboard showing:
  - Total revenue and percentage changes.
  - Revenue breakdown by category, product, and time period.
  - Top and bottom performing products.

