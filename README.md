[8:42 pm, 12/1/2026] Rupesh Reddy 💯😈: # Customer Trends & Insights Analysis (SQL | Python | Power BI)

## 📌 Project Overview
This project analyzes *customer shopping behavior* using transactional retail data to uncover trends in *spending patterns, customer segmentation, product preferences, and subscription behavior. The goal is to provide actionable insights that help stakeholders improve **sales performance, customer satisfaction, loyalty programs, and marketing strategies*.

The workflow is built as an end-to-end analytics pipeline:
- *Python* → Data cleaning, transformation, and feature engineering  
- *PostgreSQL (SQL)* → Structured business analysis through queries  
- *Power BI* → Interactive dashboard to visualize insights and trends  

---

## 🎯 Business Problem Statement
A retail company wants to better understand customer shopping behavior to improve:
- Revenue growth and conversion
- Customer engagement and satisfaction
- Long-term loyalty and subscription adoption

Management noticed changing purchase patterns across:
- Demographics (age, gender, location)
- Product categories and items
- Discounts and promotional behavior
- Review ratings and shipping preferences
- Subscription vs non-subscription customers

*Overarching Business Question:*  
> How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?

---

## 📊 Dataset Summary
- *Total Records:* 3,900 purchases  
- *Total Columns:* 18  
- *Key Features:*
  - *Customer Demographics:* Age, Gender, Location, Subscription Status
  - *Purchase Details:* Item Purchased, Category, Purchase Amount, Season, Size, Color
  - *Shopping Behavior:* Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type
- *Missing Data:* 37 values in the Review Rating column  

---

## 🧰 Tech Stack
- *Python:* pandas, numpy  
- *SQL Database:* PostgreSQL  
- *BI Tool:* Power BI  
- *Version Control:* Git & GitHub  

---

## ✅ Project Workflow

### 1) Data Preparation & Modeling (Python)
Data cleaning and transformation were performed using Python to prepare the dataset for analysis and reporting.

*Key Steps:*
- *Data Loading:* Imported dataset using pandas  
- *Initial Exploration:* df.info() and df.describe()  
- *Missing Data Handling:* Imputed missing values in review_rating using *median rating per product category*  
- *Column Standardization:* Renamed columns to *snake_case*  
- *Feature Engineering:*
  - Created age_group using age binning
  - Created purchase_frequency_days from purchase behavior data
- *Data Consistency Check:*
  - Verified redundancy between discount_applied and promo_code_used
  - Dropped promo_code_used
- *Database Integration:*
  - Connected Python workflow to PostgreSQL and loaded the cleaned dataset for SQL analysis

---

### 2) Data Analysis (SQL - PostgreSQL)
Structured SQL analysis was performed to answer critical business questions about customer behavior, loyalty, and purchase drivers.

*Key Business Questions Answered:*
1. Revenue contribution by Gender  
2. High-spending customers who used Discounts  
3. Top 5 Products by Review Rating  
4. Average purchase comparison (Standard vs Express Shipping)  
5. Subscribers vs Non-Subscribers (average spend + revenue)  
6. Discount-dependent products (highest % of discounted purchases)  
7. Customer segmentation (New / Returning / Loyal)  
8. Top 3 products per category (most purchased)  
9. Repeat buyers (>5 purchases) vs subscription likelihood  
10. Revenue contribution by Age Group  

> SQL scripts are available inside the /sql folder.

---

### 3) Visualization & Dashboard (Power BI)
Created an interactive Power BI dashboard to highlight major trends and support decision-making.

Dashboard covers:
- Revenue and purchase trends
- Customer segmentation and loyalty
- Subscription impact on revenue…
[8:42 pm, 12/1/2026] Rupesh Reddy 💯😈: Customer-Trends-Insights-Analysis/ │── data/ │   ├── raw/ │   ├── processed/ │── notebooks/ │   ├── data_cleaning_feature_engineering.ipynb │── sql/ │   ├── create_tables.sql │   ├── business_queries.sql │── powerbi/ │   ├── dashboard.pbix │── reports/ │   ├── project_report.pdf │   ├── presentation.pptx │── README.md
[8:42 pm, 12/1/2026] Rupesh Reddy 💯😈: ---

## 🚀 How to Run This Project

### Step 1: Python (Cleaning + Transformation)
1. Open Jupyter Notebook
2. Run notebook in /notebooks/
3. Export cleaned dataset to /data/processed/

### Step 2: PostgreSQL (SQL Analysis)
1. Create PostgreSQL database and tables using /sql/create_tables.sql
2. Load cleaned dataset into the database table
3. Execute analysis queries from /sql/business_queries.sql

### Step 3: Power BI Dashboard
1. Open the .pbix file from /powerbi/
2. Refresh dataset connection (CSV/SQL)
3. Use filters and slicers to explore insights

--- 
Data Analytics Project (SQL | Python | Power BI)

---
