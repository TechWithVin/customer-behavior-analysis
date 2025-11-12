🛒 Customer Shopping Behavior Analysis


🎯 Overview

Ever wondered what makes customers click “Buy Now”?
This project explores shopping behavior through 3,900 real transactions, uncovering insights about spending habits, product trends, and loyalty patterns — all backed by Python, PostgreSQL, and Power BI.

🔍 The goal:

Transform raw transaction data into actionable business insights for smarter marketing and retention strategies.

📊 Key Insights at a Glance

✅ Female customers contributed slightly more to total revenue
✅ Express shipping users tend to spend higher per transaction
✅ Loyal customers (≥5 purchases) are 2x more likely to have subscriptions
✅ Some categories rely heavily on discounts — a red flag for profitability
✅ The 25–40 age group dominates total revenue

<details> <summary>🧾 <b>Dataset Summary</b> (click to expand)</summary>
Feature Type	Description
Rows	3,900
Columns	18
Missing Values	37 in review_rating
Key Features	Age, Gender, Subscription, Purchase Amount, Category, Season, Discount, Rating, Shipping Type

📁 Categories analyzed:
Fashion, Electronics, Groceries, Beauty, Home Decor, Sports, and more.

</details>
🧹 Data Preparation (Python)

➡️ Step-by-step data wrangling:

Loaded and explored dataset with pandas

Handled missing review_rating using category-based median

Standardized columns to snake_case

Engineered new features:

age_group (binned age values)

purchase_frequency_days

Removed redundant column: promo_code_used

Integrated final dataset into PostgreSQL for SQL-based business queries

🧮 SQL Business Analysis

Here’s what we discovered using PostgreSQL:

Query	Insight
1. Revenue by Gender	Compare total revenue by male vs female
2. Discount Users	Identify customers who spend high even with discounts
3. Top 5 Products by Rating	Find the most loved products
4. Shipping Type Comparison	Standard vs Express spending habits
5. Subscribers vs Non-Subscribers	Which group brings more revenue
6. Discount-Dependent Products	Products that rely heavily on discounts
7. Customer Segmentation	New, Returning, and Loyal customers
8. Top 3 Products per Category	Discover category champions
9. Repeat Buyers vs Subscription	Does loyalty drive subscriptions?
10. Revenue by Age Group	Which age group drives revenue the most
📈 Power BI Dashboard

💡 An interactive dashboard was created in Power BI to visualize:

Total revenue by gender, age, and subscription status

Product performance and rating

Discount dependency per product

Shipping trends and purchase frequency

🎥 (Optional: Add a dashboard screenshot or GIF preview here)

💼 Business Recommendations

💬 Data tells a story — here’s what we learned:

Strategy	Action
Boost Subscriptions	Offer exclusive benefits and perks
Loyalty Program	Reward returning buyers
Discount Review	Balance between conversion and profit margin
Top-Rated Products	Prioritize in ads and placement
Targeted Marketing	Focus on high-value age segments and express users
⚙️ Tools & Technologies
Category	Tools
Programming	Python (pandas, numpy, matplotlib, seaborn)
Database	PostgreSQL
Visualization	Power BI
Version Control	Git & GitHub
