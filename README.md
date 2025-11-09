# Credit Score Analysis — Power BI with Python Integration

## Overview

This project explores how data cleaning, transformation, and visualization come together to assess customer credit behavior. Using Power BI for analytics and Python within Power Query, it demonstrates how businesses can classify customers by credit health, monitor repayment performance, and identify potential risks in their portfolio.

The visuals and insights are built from real analytical logic — the report provides an intuitive way to understand customer distribution, payment delays, and credit quality segments. Everything you see in the dashboard has been automated through a clean, transparent data pipeline.

## Project Objective

To evaluate credit score performance and repayment behavior across thousands of customers, giving financial institutions or analysts a way to:

Detect at-risk customers early based on payment delays.

Identify top-quality segments with strong repayment history.

Measure income-to-debt performance and credit utilization.

Present KPIs and distribution metrics through a visually rich, interactive Power BI dashboard.

## Tools & Technologies

| Tool                    | Purpose                                                                           |
| ----------------------- | --------------------------------------------------------------------------------- |
| **Power BI**            | Dashboard design, KPI visualization, and DAX measures                             |
| **Power Query**         | Data extraction, transformation, and integration                                  |
| **Python**              | Advanced data cleaning, handling missing values, standardizing numeric formats    |
| **Excel / CSV Dataset** | Input source for customer data                                                    |
| **DAX**                 | Creating calculated measures for category segmentation and performance comparison |


## Data Cleaning with Python in Power Query

A key highlight of this project is the Python-based data cleaning pipeline executed inside Power Query. Instead of manual transformations, Python automates the following:

Fixing data types — converting numeric and date columns to the correct format.

Removing duplicates — ensuring each Customer ID is unique per month.

Handling missing values — replacing nulls in numeric columns with medians and in text columns with “Missing”.

Standardizing column formats — consistent casing, trimming extra spaces, and unifying field types.

Deriving new metrics — including Credit Health Index, Payment Delay, and Outstanding Debt Ratios.

This hybrid approach allows Power BI to leverage Python’s flexibility for preprocessing and Power BI’s DAX for analytical logic.


## Dashboard Highlights

![My Project Screenshot](https://i.ibb.co/4ZF5ZXgg/credit-score-analysis-page-0001-1.jpg).
### 1. KPI Card Section

Provides an instant overview of key metrics:

Average Monthly Income (AED): 4.08K

Average Credit Score: 0.90

Total Customers: 11.81K

Average Outstanding Debt (AED): 1.39K

Top Credit Quality Segment: 5,193

At-Risk Segment: 678

### 2. Payment Delay Analysis

Bar charts visualize how average payment delays vary across customer categories:

Watchlist – 46 days

Standard – 33 days

Good – 24 days

Excellent – 13 days

This instantly highlights risk zones where collection teams should focus attention.

### 3. Credit Health Distribution

Displays how customers are spread across different health categories:

Standard: 5.9K

Good: 4.8K

Watchlist: 0.7K

Excellent: 0.4K

### 4. Customer Detail View

A tabular view listing every customer’s credit profile:
| Customer ID | Credit Health Category | Credit Health Index | Payment Delay (Days) | Monthly Income (AED) |
| ----------- | ---------------------- | ------------------- | -------------------- | -------------------- |
| CUS_0x1009  | Good                   | 0.62                | 234.25               | 4,250.39             |

It’s designed for drill-through analysis — perfect for analysts who need to inspect individual records contributing to KPI trends.
Business Insights

The Watchlist group shows the longest delays (46 days), requiring focused risk mitigation.

The Standard and Good segments form the largest customer base, representing stable contributors to overall credit performance.

The Excellent group, though small, indicates strong repayment behavior and low credit risk.

The average credit score (0.90) shows generally positive customer health but still signals an opportunity for improvement in timely payments.

## Learnings & Impact

This project shows how easily Power BI can integrate Python scripts for deep data preparation without leaving the BI environment. It highlights how clean data directly enhances visualization accuracy, helping decision-makers trust their dashboards.

Whether you are a data analyst, business manager, or finance professional, this project is a model for building an analytics workflow that combines:

Automation (Python)

Visualization (Power BI)

Business logic (DAX)
