# CUSTOMER-BEHAVIOR-ANALYSIS
Customer Shopping Behavior Analysis
📌 Project Overview

This project focuses on analyzing customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The objective is to uncover actionable insights related to customer demographics, spending patterns, product performance, discount usage, and subscription behavior to support data-driven business decisions.

🎯 Business Objectives

Understand customer purchasing and spending patterns

Identify high-value customer segments

Analyze the impact of discounts and subscriptions

Evaluate product performance and customer satisfaction

Support strategic decisions through data visualization

📂 Dataset Summary

Total Records: 3,900

Total Columns: 18

Data Type: Transactional retail data

Key Features

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Behavioral Metrics:

Discount Applied

Promo Code Used

Previous Purchases

Purchase Frequency

Review Rating

Shipping Type

Data Quality

Missing values: 37 entries in the Review Rating column

All missing values were handled during preprocessing

🐍 Exploratory Data Analysis (Python)

EDA and data preparation were conducted using Python.

Key Steps

Data Loading: Imported data using pandas

Initial Exploration:

df.info() for structure

df.describe() for summary statistics

Missing Value Handling:

Imputed missing Review Rating values using the median rating per product category

Column Standardization:

Converted column names to snake_case

Feature Engineering:

Created age_group by binning customer ages

Derived purchase_frequency_days

Data Consistency Check:

Identified redundancy between discount_applied and promo_code_used

Dropped promo_code_used

Database Integration:

Loaded the cleaned dataset into PostgreSQL for SQL analysis

🗄️ Data Analysis Using SQL (PostgreSQL)

Structured SQL queries were written to answer real-world business questions:

Revenue comparison by gender

Identification of high-spending customers using discounts

Top 5 products by average review rating

Comparison of purchase amounts by shipping type

Spend analysis: Subscribers vs Non-Subscribers

Products most dependent on discounts

Customer segmentation (New, Returning, Loyal)

Top 3 products within each category

Relationship between repeat purchases and subscription status

Revenue contribution by age group

📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize:

Revenue trends

Customer segmentation

Product performance

Subscription behavior

Discount impact

This dashboard enables stakeholders to quickly interpret insights and make informed decisions.

💡 Business Recommendations

Based on the analysis:

Boost Subscriptions:
Promote exclusive benefits for subscribers

Strengthen Loyalty Programs:
Incentivize repeat purchases to convert customers into the “Loyal” segment

Optimize Discount Strategy:
Balance discount usage with profit margins

Improve Product Positioning:
Highlight top-rated and best-selling products

Targeted Marketing:
Focus on high-revenue age groups and express-shipping users

🛠️ Tools & Technologies

Python: Pandas, NumPy, Matplotlib, Seaborn

SQL: PostgreSQL

BI Tool: Power BI

IDE: Jupyter Notebook / VS Code
