# Roxelle
Data analytics project work

produced by: Abraham Ogboli Osefumnanya

1. Project Overview
Roxelle Nigeria Ltd. Sales & Operations Analytics Dashboard

This project was developed as part of the Power BI Final Year Capstone Assignment. The objective was to transform transactional and operational data from Roxelle Nigeria Ltd. into an interactive business intelligence solution that supports data-driven decision-making.

The dashboard analyzes sales performance, customer behaviour, product performance, and discount effectiveness across six branches located in Lagos and Abuja.

2. Business Problem

Roxelle Nigeria Ltd. faced several business challenges including:

Limited visibility into branch-level performance
Uncontrolled discount spending
High product return rates
Inefficient product stocking decisions
Lack of customer behaviour insights

This Power BI solution was designed to address these challenges through interactive reporting and analytical dashboards.

3. Dataset Description

The analysis was conducted using five CSV datasets:

Dataset	Description
sales_transactions	Transaction-level sales records
customers	Customer demographic and loyalty information
products	Product details, categories and pricing
branches	Branch information and locations
date	Calendar table for time intelligence analysis

4. Power Query Transformations

The following transformations were performed in Power Query:

Loaded all five CSV files into Power BI
Renamed columns to improve readability
Assigned appropriate data types to all fields
Handled null and blank values where applicable
Created Revenue After Discount column
Removed duplicate records
Verified data quality before loading into the model
Revenue After Discount Formula
Revenue After Discount =
Quantity × Unit Price × (1 - Discount Percent / 100)

5. Data Model Design

A star schema was implemented to improve performance and simplify analysis.

Relationships
Customers → Sales Transactions
Products → Sales Transactions
Branches → Sales Transactions
Date → Sales Transactions
Cross Filter Direction

Single-direction filtering was used throughout the model.

Reason:
Single-direction relationships improve model performance, reduce ambiguity, and prevent unwanted filter propagation.
One-to-many relationships were used in the model.

6. DAX Measures

The following measures were created:

Total Revenue	Total revenue after discounts
Total Cost	Total product cost
Total Profit	Revenue minus cost
Profit Margin %	Profitability percentage
Total Transactions	Distinct transaction count
Return Rate %	Percentage of returned transactions
Avg Basket Size	Revenue per transaction
MoM Revenue %	Month-over-month revenue growth
Average Discount %	Average discount percentage applied

Additional Measure Justification:
Average Discount % was created to evaluate the effectiveness of promotional activities and support discount audit analysis.

7. Dashboard Pages
Page 1 – Sales Performance

Provides visibility into:

Revenue
Profit
Profit Margin
Branch Performance
Sales Trends
Category Contribution

Page 2 – Customer Behaviour

Provides insights into:

Customer Segments
Loyalty Programme Performance
Customer Demographics
Geographic Distribution
Average Basket Size

Page 3 – Product Performance

Provides insights into:

Top and Bottom Products
Product Return Rates
Category Profitability
Product Contribution Analysis

Page 4 – Discount Audit

Provides insights into:

Discount Impact
Branch Discount Activity
Discount Effectiveness
Basket Size Analysis
Payment Method Behaviour
8. Key Insights & Recommendations
Key Findings
Surulere Branch generated the highest revenue contribution.
Food & Beverages was the strongest-performing product category.
Loyalty customers demonstrated stronger purchasing behaviour.
Several products exhibited elevated return rates.
Discounts increased basket size but did not always result in proportional revenue growth.
Recommendations
Increase focus on high-performing product categories.
Review low-performing and high-return products.
Expand loyalty programme adoption.
Optimize discount policies across branches.
Continue monitoring profitability alongside revenue growth.

9. Power BI Service Link
Published Dashboard:
Publishing could not be completed due to lack of access to a Microsoft organizational account.

10. Repository Contents

datasets/
sales_transactions.csv
customers.csv
products.csv
branches.csv
date.csv

screenshots/
sales_performance.png
customer_behaviour.png
product_performance.png
discount_audit.png
data_model.png

Roxelle_Capstone.pbix

summary.pdf

README.md

summary.pdf
README.md
