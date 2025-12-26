🛒 Customer Shopping Behavior Analysis
📌 Project Overview

This project focuses on analyzing customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The objective is to uncover insights related to spending patterns, customer segmentation, product preferences, discounts, subscriptions, and revenue trends to support data-driven business decisions.

📊 Dataset Summary

Total Records: 3,900

Total Features: 18

Data Type: Transactional retail data

Key Attributes:

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Behavioral Metrics:

Discount Applied

Previous Purchases

Purchase Frequency

Review Rating

Shipping Type

Data Quality:

Missing values found in the Review Rating column

Missing values were handled using median imputation per product category

🧹 Data Cleaning & Preprocessing (Python)

The dataset was cleaned and prepared using Python:

Loaded data using pandas

Performed structural inspection using .info() and .describe()

Handled missing values in review ratings using median-based imputation

Renamed columns to snake_case for consistency

Performed feature engineering:

Created age_group feature

Derived purchase_frequency_days

Identified redundant features and removed promo_code_used

Exported cleaned data to PostgreSQL for SQL-based analysis

🗄️ Database & SQL Analysis (PostgreSQL)

The cleaned dataset was loaded into PostgreSQL to answer real-world business questions using SQL.

Key Business Analyses:

Revenue by Gender

High-Spending Discount Users

Top 5 Products by Average Rating

Shipping Type vs Average Purchase Amount

Subscribers vs Non-Subscribers Revenue Comparison

Discount-Dependent Products

Customer Segmentation (New, Returning, Loyal)

Top 3 Products per Category

Repeat Buyers vs Subscription Status

Revenue Contribution by Age Group

Advanced SQL concepts used:

Aggregations (SUM, AVG, COUNT)

CASE WHEN logic

Window functions

Grouping & filtering

Ranking queries

📈 Data Visualization (Power BI)

An interactive Power BI dashboard was developed to visualize insights, including:

Total customers and average purchase amount

Revenue distribution by category and age group

Subscription vs non-subscription comparison

Shipping type impact

Customer segmentation insights

The dashboard enables business stakeholders to quickly understand customer behavior patterns.

💡 Key Insights

Male customers generated higher total revenue

Express shipping users spent slightly more on average

Non-subscribers contributed higher overall revenue due to volume

Loyal customers formed the largest customer segment

Certain products showed strong dependency on discounts

Young adults contributed the highest revenue among age groups

📌 Business Recommendations

Promote subscription plans with exclusive benefits

Introduce loyalty programs to retain repeat customers

Optimize discount strategies to protect profit margins

Highlight top-rated and best-selling products in campaigns

Focus marketing efforts on high-revenue age groups

Encourage express shipping for higher-value orders

🛠️ Tools & Technologies Used

Python (Pandas, NumPy)

PostgreSQL

SQL

Power BI

Jupyter Notebook

📂 Project Structure (Suggested)
├── data/
│   └── customer_shopping_data.csv
├── notebooks/
│   └── data_cleaning_analysis.ipynb
├── sql/
│   └── business_queries.sql
├── powerbi/
│   └── customer_behavior_dashboard.pbix
├── README.md

🚀 Conclusion

This project demonstrates an end-to-end data analytics workflow, combining Python, SQL, and BI tools to transform raw transactional data into actionable buiness insights. It reflects real-world analytical problem-solving and decision-support capabilities.
