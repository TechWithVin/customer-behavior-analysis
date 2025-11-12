🛍️ Customer Shopping Behavior Analysis
📖 Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories.
The main goal is to uncover spending patterns, customer segments, product preferences, and subscription behavior to support data-driven business decisions.

🧾 Dataset Summary
Feature Type	Description
Rows	3,900
Columns	18
Key Features	Customer demographics, purchase details, and shopping behavior
Missing Data	37 missing values in review_rating column
Key Attributes

Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Amount, Season, Size, Color

Behavioral Features: Discount Applied, Promo Code Used, Frequency of Purchases, Review Rating, Shipping Type

🧹 Data Preparation (Python)

Main steps conducted in Python (Pandas):

Data Loading: Imported dataset using pandas

Exploration: Used df.info() and df.describe() for data overview

Missing Data Handling: Filled missing review ratings with median per category

Column Standardization: Renamed columns to snake_case

Feature Engineering:

Created age_group by binning ages

Created purchase_frequency_days

Redundancy Check: Dropped promo_code_used (redundant with discount_applied)

Database Integration: Loaded cleaned data into PostgreSQL for SQL analysis

🧮 SQL Analysis (PostgreSQL)

Performed SQL-based analysis to extract business insights:

Revenue by Gender – Compare male vs female revenue

High-Spending Discount Users – Customers using discounts but spending above average

Top 5 Products by Rating – Highest average review scores

Shipping Type Comparison – Standard vs Express average purchase

Subscribers vs Non-Subscribers – Revenue and spending comparison

Discount-Dependent Products – Products with the highest discount usage

Customer Segmentation – Classify into New, Returning, and Loyal customers

Top 3 Products per Category – Identify most-purchased items per category

Repeat Buyers & Subscriptions – Correlation between frequency and subscriptions

Revenue by Age Group – Total revenue by age segment

📊 Power BI Dashboard

A fully interactive Power BI dashboard was developed to visualize:

Revenue distribution

Top products

Subscription patterns

Customer segmentation

Shipping preferences

💡 Business Recommendations

Boost Subscriptions: Offer exclusive benefits to increase sign-ups

Customer Loyalty Program: Reward repeat buyers to increase retention

Review Discount Policy: Ensure discounts improve sales without hurting profit

Product Positioning: Highlight top-rated and high-performing products

Targeted Marketing: Focus on high-revenue age groups and express-shipping users

🧰 Tools Used

Python: pandas, numpy, matplotlib, seaborn

Database: PostgreSQL

Visualization: Power BI

Version Control: Git & GitHub
