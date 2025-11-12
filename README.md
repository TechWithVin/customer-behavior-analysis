# 🛒 Customer Shopping Behavior Analysis  

[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-316192?logo=postgresql)](https://www.postgresql.org/)
[![Power BI](https://img.shields.io/badge/Visualization-PowerBI-F2C811?logo=powerbi)](https://powerbi.microsoft.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Made by Kevin](https://img.shields.io/badge/Made%20by-Kevin%20Zakky-red?logo=github)](#author)

---

## 🎯 Overview  

Ever wondered what makes customers **click “Buy Now”?**  
This project explores **shopping behavior** through **3,900 real transactions**, revealing insights on **spending patterns, product trends, and loyalty behavior** — all analyzed using **Python**, **PostgreSQL**, and **Power BI**.

> 🎯 Goal: Transform raw transaction data into actionable business insights for smarter marketing and retention strategies.

---

## 📊 Dashboard Preview  

<p align="center">
  <img src="images/dashboard_preview.png" alt="Power BI Dashboard Preview" width="800"/>
  <br>
  <em>Interactive Power BI dashboard showing customer segmentation, revenue by age group, and top-rated products.</em>
</p>

---

## 🧾 Dataset Summary  

| Feature | Description |
|----------|-------------|
| **Rows** | 3,900 |
| **Columns** | 18 |
| **Missing Values** | 37 in `review_rating` |
| **Key Features** | Age, Gender, Subscription, Purchase Amount, Category, Season, Discount, Rating, Shipping Type |

📂 **Categories included:** Fashion, Electronics, Groceries, Beauty, Home Decor, Sports, and more.

---

## 🧹 Data Preparation (Python)  

**Steps performed in Jupyter Notebook:**
- Loaded dataset using `pandas`
- Filled missing values in `review_rating` using median per category
- Standardized column names → `snake_case`
- Created new features:
  - `age_group` (binned by customer age)
  - `purchase_frequency_days`
- Dropped redundant `promo_code_used` column  
- Integrated cleaned data into **PostgreSQL** for further SQL analysis  

---

## 🧮 SQL Business Analysis  

| # | Analysis | Description |
|---|-----------|-------------|
| 1 | **Revenue by Gender** | Compare total revenue by male vs female customers |
| 2 | **High-Spending Discount Users** | Customers who use discounts but spend above average |
| 3 | **Top 5 Products by Rating** | Identify products with the highest average review |
| 4 | **Shipping Type Comparison** | Compare standard vs express shipping averages |
| 5 | **Subscribers vs Non-Subscribers** | Revenue and average spend by subscription status |
| 6 | **Discount-Dependent Products** | Products relying most on discounts |
| 7 | **Customer Segmentation** | Group into New, Returning, and Loyal segments |
| 8 | **Top 3 Products per Category** | Most purchased products by category |
| 9 | **Repeat Buyers & Subscriptions** | Check correlation between repeat purchase and subscription |
| 10 | **Revenue by Age Group** | Total revenue by customer age segments |

---

## 📈 Power BI Dashboard Insights  

🎨 **Visualized in Power BI** for intuitive understanding of:  
- Revenue distribution by gender, age, and location  
- Product ratings and discount utilization  
- Customer segmentation & subscription patterns  
- Purchase frequency and shipping type preferences  

---

## 💡 Business Recommendations  

| Focus Area | Recommendation |
|-------------|----------------|
| **Boost Subscriptions** | Offer exclusive perks and loyalty rewards |
| **Customer Retention** | Implement a points-based loyalty system |
| **Discount Strategy** | Optimize discount campaigns to maintain margin |
| **Product Positioning** | Highlight top-rated and best-selling items |
| **Targeted Marketing** | Focus campaigns on high-revenue segments and express users |

---

## ⚙️ Tools & Technologies  

| Category | Tools |
|-----------|-------|
| **Programming** | Python (pandas, numpy, matplotlib, seaborn) |
| **Database** | PostgreSQL |
| **Visualization** | Power BI |
| **Version Control** | Git & GitHub |

---

## 📂 Repository Structure  

```bash
├── data/
│   └── customer_shopping_behavior.csv
├── notebooks/
│   └── data_cleaning_and_eda.ipynb
├── sql/
│   └── analysis_queries.sql
├── dashboard/
│   └── powerbi_dashboard.pbix
├── images/
│   └── dashboard_preview.png
├── README.md
└── requirements.txt
