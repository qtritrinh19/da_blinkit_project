# Blinkit Retail Sales & Revenue Analysis: An End-to-End Data Analytics Project

This project showcases a complete end-to-end data analytics workflow, from processing raw data to building an interactive Power BI dashboard. It aims to solve a real-world business case focused on analyzing sales performance for Blinkit.

##  1. Business Context & Objectives

The primary goal of this project is to transform raw sales data into actionable insights that empower leadership to make strategic, data-driven decisions. Based on the revenue analysis for October 2024, we aim to answer the following core business questions:

* **Overall Business Health:** Are we in a state of growth or decline?
* **Growth Drivers:** Which categories and products are generating the most revenue?
* **Potential Risks:** Which categories and products are underperforming and require immediate attention?
* **Strategic Actions:** What short-term and long-term strategies should be implemented to optimize revenue?

##  2. Interactive Power BI Dashboard

The final output of the analysis pipeline is a dynamic dashboard designed for end-users (like Sales Managers and the Marketing Team) to easily monitor and explore key insights.

![Dashboard](/image/Blintit_Dash.png)

**Key Features:**

* **High-Level KPIs:** Instantly track critical metrics such as total revenue, which hit **$255.9K**, a strong Month-over-Month (MoM) growth of **+10.75%**, but also a concerning Year-over-Year (YoY) decline of **-3.03%**.
* **In-Depth Analysis:** Drill down into the performance of each category, highlighting the outstanding **+95.86%** MoM growth of "Dairy & Breakfast" and the alarming **-50.65%** MoM decline of "Personal Care".
* **Dynamic Filtering:** Users can flexibly filter the report by date, month, year, or specific product categories.
* **Top/Bottom Performers:** Automatically identifies best-selling products (like **Butter, Bread, and Pet Treats**) and products with the sharpest revenue drops (like **Toothpaste and Cough Syrup**) to inform marketing and inventory strategies.

##  3. Detailed Analysis & Strategic Recommendations

Based on the data, the project has identified key growth drivers and risks, leading to specific, actionable recommendations.

### Business Health: Short-Term Gain vs. Long-Term Pain

While this month saw a strong recovery with a **+10.75% MoM revenue increase**, it masks a persistent negative long-term trend, with revenue down **-3.03%** compared to the same time last year. This indicates that the short-term gains are not yet enough to reverse the concerning long-term trajectory.

### Growth Drivers 

* **Dairy & Breakfast:** The top-performing category with **$47.2K in revenue** and an outstanding MoM growth of **+95.86%**, driven primarily by its core products, **Butter and Bread**.
* **Pet Care:** A strong contender with **$33.1K in revenue** and **+50.16% MoM growth**, with **Pet Treats** being the main driver.
* **Fruits & Vegetables** and **Grocery & Staples** also demonstrated solid, stable growth.

### Key Risks 

* **Personal Care:** The biggest risk category, experiencing a significant **-50.65% MoM decline**. This issue is concentrated in one specific product, **Toothpaste**, which saw a sharp revenue drop of **-$7,816**.
* **Pharmacy:** Showed a considerable **-28.27% MoM decrease**, confirming a broader trend of decline within the category, led by **Cough Syrup and Vitamins**.
* **Hidden Risk:** Even within the high-growth "Dairy & Breakfast" category, the product **Cheese** is struggling, with a revenue decline of **-$3,741**. This highlights the need for product-level monitoring.

### Strategic Recommendations

A two-pronged strategy is proposed: (1) Amplify growth in top-performing categories and (2) Intervene to mitigate risks in declining categories.

* **Short-Term Strategy:**
    * **Growth:** Launch targeted marketing campaigns for **Butter, Bread, and Pet Treats**. Introduce special bundle deals for **Grocery & Staples**.
    * **Risk Mitigation:** Conduct a quick market analysis to understand the decline of **Toothpaste**. Initiate promotional campaigns with discounts on **Cough Syrup and Vitamins**.
* **Long-Term Strategy:**
    * Conduct a thorough competitive analysis of competitors' pricing, marketing, and product portfolios.
    * Perform a market needs assessment through customer surveys to ensure product offerings meet current demand.

##  4. Technical Architecture & ETL Workflow

The project is built on a clear and automated ETL (Extract - Transform - Load) pipeline.

`Raw Data (.csv)` -> `Processing & Cleaning (Python)` -> `Storage (MS SQL Server)` -> `Visualization (Power BI)`

1.  **Extract & Transform (Python):**
    * Utilized the **Pandas** library to read and process the raw `.csv` file.
    * Key data cleaning steps included removing duplicates, standardizing date formats, and handling missing values.
2.  **Load (MS SQL Server):**
    * Used **SQLAlchemy** to create a connection engine between Python and MS SQL Server.
    * The cleaned data from the Pandas DataFrame was loaded into a table in SQL Server, simulating a real-world environment where data is managed centrally and securely.
3.  **Visualize (Power BI):**
    * Connected Power BI directly to the MS SQL Server database.
    * Built charts, measures, and calculated columns using **DAX** to derive meaningful insights from the data.

##  5. Technology Stack

* **Programming Language:** `Python 3`
* **Python Libraries:** `Pandas`, `SQLAlchemy`
* **Database:** `Microsoft SQL Server`
* **Business Intelligence:** `Microsoft Power BI`

---
Thank you for checking out this project!
