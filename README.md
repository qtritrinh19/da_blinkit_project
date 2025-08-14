# **Blinkit Retail Sales & Revenue Analysis with Power BI and SQL**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SQL Server](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

This project showcases a complete end-to-end data analytics workflow, from raw data to an interactive dashboard, solving a real-world business case for sales performance analysis.

**(IMPORTANT) View the live, interactive dashboard here: [Link to your Public Power BI Dashboard]**

## 🎯 **Project Objectives & Business Context**

The goal of this project extends beyond technical practice. It aims to answer core business questions for an e-commerce platform like Blinkit:
* Which products and categories are the top revenue generators?
* How do sales trends evolve over time?
* How can we identify growth opportunities and potential risks from sales data?

This project simulates a real-world environment where data is processed, stored, and visualized to support data-driven business decisions.

## ✨ **Interactive Dashboard Showcase - Power BI**

The dashboard is the final product of the analysis pipeline, designed for end-users (like Sales Managers or the Marketing Team) to easily interact with and explore insights.

*[Insert a high-quality GIF or screenshot of your dashboard here. This is the most critical part for making a great first impression!]*

**Key Features of the Dashboard:**
* **High-Level KPIs:** Track total revenue, Month-over-Month/Year-over-Year growth, and other critical metrics at a glance.
* **Category-Specific Analysis:** Interactive charts allow for a deep dive into the revenue performance of each product category.
* **Dynamic Filtering:** Users can dynamically filter the report by date, month, year, or specific product categories.
* **Top/Bottom Performers:** Automatically identifies best-selling and worst-selling products to inform inventory and marketing strategies.

## 🏗️ **Technical Architecture & Workflow**

The project is built on a clear and automated ETL (Extract - Transform - Load) pipeline.

`Raw Data (.csv)` -> `Processing & Cleaning (Python)` -> `Storage (MS SQL Server)` -> `Visualization (Power BI)`

**1. Extract & Transform (Python):**
* Utilized the **Pandas** library to read and process the raw `.csv` file from Kaggle.
* **Key data cleaning steps:**
    * Removed duplicate and invalid entries.
    * Standardized date formats to ensure consistency.
    * Handled missing values where applicable.
* The Python script is designed to be reusable for new datasets with a similar structure.

**2. Load (MS SQL Server):**
* Used **SQLAlchemy** to create a connection engine between Python and MS SQL Server, a common solution in enterprise applications.
* The cleaned data from the Pandas DataFrame was loaded into a table in SQL Server using the `to_sql()` method.
* Storing data in SQL Server simulates a real-world environment where data is managed centrally and securely, ready for various analytics tools to connect to it.

**3. Visualize (Power BI):**
* Connected Power BI directly to the MS SQL Server database using **DirectQuery** or **Import** mode for optimal performance and data freshness.
* Built charts, measures, and calculated columns using **DAX** to derive meaningful insights from the raw data.

## 🛠️ **Technology Stack**

* **Programming Language:** `Python 3.x`
* **Python Libraries:** `Pandas`, `SQLAlchemy`
* **Database:** `Microsoft SQL Server`
* **Business Intelligence:** `Microsoft Power BI`

## 🚀 **Installation & Usage**

To run this project on your local machine, please follow these steps:

**Prerequisites:**
* Python 3.x
* MS SQL Server installed and running.
* Power BI Desktop.

**Steps:**
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```
2.  **Create a virtual environment and install dependencies:**
    ```bash
    python -m venv venv
    venv\Scripts\activate  # On Windows
    # source venv/bin/activate  # On macOS/Linux
    pip install -r requirements.txt
    ```
3.  **Configure the Database:**
    * Open the Python script (`your_script_name.py`).
    * Update the database connection string with your MS SQL Server credentials.
4.  **Run the ETL script:**
    ```bash
    python your_script_name.py
    ```
5.  **Open the Power BI report:**
    * Open the `.pbix` file using Power BI Desktop.
    * If prompted, update the data source credentials in Power Query to connect to your local SQL Server instance.

---
Thank you for checking out this project!
