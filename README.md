# Sales Data Analysis & Customer Insight Project


# 1. Business Framing

## Problem Statement

The business is currently facing several challenges in its sales and customer management system:

* Negative profit observed in multiple transactions
* Lack of visibility into top-performing products
* No customer segmentation to identify high-value customers
* Inefficient promotional strategies


## Objectives

* Improve overall profitability
* Identify top-performing and loss-making products
* Segment customers based on behavior and value
* Provide actionable recommendations for business growth


# 2. Data Understanding & Preparation

## Dataset Overview

* Source: Sales dataset (Excel)
* Size: Approximately 900 rows
* Key Features:

  * Product (Hàng, Mã)
  * Revenue (Doanh Thu)
  * Cost (Tiền Nhập)
  * Profit (PROFIT)
  * Quantity (SL Xuất, SL Xuất KM)
  * Date (Ngày Xuất, MONTH, YEAR)
  * Customer (Khách hàng)


## Data Cleaning

* Converted date columns to proper datetime format
* Removed invalid and inconsistent records
* Checked for:

  * Negative or abnormal profit values
  * Missing or zero quantities
* Created new features:

  * Profit = Revenue - Cost
  * Total Quantity = SL Xuất + SL Xuất KM


## Exploratory Data Analysis (EDA)

### Time-based Analysis

* Monthly revenue trend
* Identification of peak sales periods

### Product Analysis

* Top-performing products by revenue
* Loss-making products impacting profit

### Customer Analysis

* Top customers by revenue contribution
* Distribution of customer purchasing behavior


## Data Modeling (ERD)

Entity Relationship Diagram:

```
Customer ──< Orders ──< OrderDetails >── Product
```

## SQL Techniques Used

* CTE (Common Table Expressions)
* Window Functions (ROW_NUMBER, RANK, SUM OVER)


# 3. Customer Segmentation (RFM Analysis)

## RFM Model

* Recency: How recently a customer purchased
* Frequency: How often they purchase
* Monetary: How much they spend


## Segmentation Results

* VIP Customers: High frequency and high spending
* Regular Customers: Moderate engagement
* Churn Risk: Low activity and low value


## Business Value

* Personalized offers for VIP customers
* Re-engagement campaigns for churn-risk customers
* Improved customer retention strategy


# 4. Recommendation System

## Key Insights

* Several products generate high revenue but negative profit
* A small number of products contribute to most revenue
* A minority of customers drive the majority of sales


## Recommendations

* Discontinue or reprice loss-making products
* Focus marketing efforts on top-performing products
* Implement loyalty programs for VIP customers
* Optimize promotion strategy to improve profitability


# 5. Dashboard & Presentation

## Dashboard Overview

The dashboard provides a comprehensive view of:

* Total Revenue
* Total Profit
* Total Quantity Sold
* Revenue trends over time
* Top products
* Top customers


## Features

* Interactive filters (Date, Product, Customer)
* Dynamic charts and KPIs
* Drill-down capabilities


## Data Storytelling Flow

1. Problem Identification
2. Data Overview
3. Analysis
4. Insights
5. Recommendations


# Conclusion

This project demonstrates how data analysis can:

* Transform raw sales data into actionable insights
* Identify critical business issues
* Support strategic decision-making


# Tools Used

* Excel (Pivot Tables)
* Power BI (Dashboard)
* SQL (Data Analysis)
* Python (Optional for advanced analysis)


