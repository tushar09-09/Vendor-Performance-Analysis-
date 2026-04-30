Vendor Performance Analysis
🔍 Overview

This project focuses on analyzing vendor performance using real-world business metrics to help organizations optimize procurement, reduce costs, and improve profitability.

The system integrates multiple data sources such as purchases, sales, and vendor invoices to generate actionable insights about vendor efficiency, inventory utilization, and pricing strategies.

🎯 Business Objective

Organizations often struggle to answer critical questions such as:

Which vendors are actually profitable?
Where is money being wasted in procurement?
Which products are overstocked or underperforming?
Does bulk purchasing reduce costs effectively?

This project addresses these challenges by building a data-driven vendor evaluation system.

🧱 Project Architecture

The project is designed as a data pipeline:

CSV Data → SQLite Database → SQL Transformation → Feature Engineering → Analysis → Power BI Dashboard
⚙️ Tools & Technologies
Python (Pandas, NumPy) – Data cleaning & transformation
SQLite + SQL (CTEs) – Data modeling and aggregation
SQLAlchemy – Database ingestion automation
Power BI – Data visualization and dashboarding
Logging Module – Pipeline monitoring & debugging
🔄 Workflow
1. Data Ingestion
Loaded multiple CSV datasets (sales, purchases, invoices, pricing)
Automated ingestion into SQLite database using Python
Designed for scalability (can be extended to real-time data)
2. Data Transformation (SQL)
Used Common Table Expressions (CTEs) to modularize queries
Created intermediate summaries:
Purchase Summary
Sales Summary
Freight Cost Summary
Joined datasets to build a vendor-level performance table
3. Data Cleaning & Feature Engineering
Handled missing values and data inconsistencies
Standardized formats and removed noise
Created key business metrics:
Gross Profit
Profit Margin (%)
Stock Turnover
Sales-to-Purchase Ratio
4. Exploratory Data Analysis (EDA)
Identified trends, outliers, and anomalies
Evaluated vendor-wise and product-wise performance
Analyzed distribution of sales, costs, and margins
5. Business Analysis

Key questions answered:

Which vendors generate high revenue but low profit?
Which vendors contribute most to procurement cost?
Where is inventory stuck (low turnover)?
What is the impact of bulk purchasing on pricing?
How dependent is the business on top vendors?
6. Dashboard (Power BI)
Built an interactive dashboard for decision-makers
Key features:
Vendor performance ranking
Profitability analysis
Inventory efficiency tracking
Purchase vs Sales comparison
📈 Key Insights
Identified vendors with high sales but low profitability
Detected slow-moving inventory, leading to capital blockage
Found pricing inefficiencies in bulk purchases
Highlighted vendor dependency risks
💡 Business Impact

This project enables organizations to:

Optimize vendor selection
Reduce unnecessary procurement costs
Improve inventory management
Increase overall profitability
🧪 Challenges & Learnings
Managing joins across multiple datasets without data duplication
Designing efficient SQL queries using CTEs
Ensuring data consistency across different sources
Translating raw data into business insights

  ### 4. 📉 Power BI Dashboard

![image](https://github.com/user-attachments/assets/07a32b68-783a-4a5a-abd8-19811b13974a)

![image](https://github.com/user-attachments/assets/ed666aa2-e286-442e-93f3-b567e1f03bf8)
