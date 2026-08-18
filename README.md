# Retail Sales & Performance Analysis Dashboard

An interactive **Power BI sales analytics dashboard** designed to analyze retail performance across products, customers, promotions, sales periods, and geographic locations.

The project focuses on transforming transactional sales data into actionable business insights using **Power BI, Power Query, DAX, and dimensional data modeling**.

---

## Dashboard Preview

### Executive Sales Overview

![Sales Trends Dashboard](Report%20Screenshots/sales-overview.png)

### Product Performance Analysis

![Product Performance Dashboard](Report%20Screenshots/top-bottom-5-products.png)

### Period Comparison

![Period Comparison Dashboard](Report%20Screenshots/sales-profit-unitssold-by-datewindow.png)

### Transaction-Level Analysis

![Transaction Analysis](Report%20Screenshots/transaction-level-analysis.png)

### Data Model

![Power BI Data Model](Report%20Screenshots/data-model.png)

---

## Business Objective

The objective of this project is to build an interactive business intelligence solution that helps stakeholders understand:

* Overall sales and profitability performance
* Best- and worst-performing products
* Sales and unit volume trends
* Customer and transaction-level performance
* Promotion effectiveness
* Geographic sales distribution
* Performance differences between selected time periods

The dashboard is designed to support both **high-level management reporting** and **detailed transaction-level analysis**.

---

## Key Business Questions

The report addresses questions such as:

1. What are the highest- and lowest-performing products by sales?
2. Which products sell the highest number of units?
3. Which products generate the highest profit?
4. How do sales change over time?
5. How does performance differ between two selected periods?
6. Which cities contribute the most to net sales?
7. Which promotions provide the highest discount value?
8. How are profit and net sales related?
9. Which products or transactions contribute most significantly to overall revenue?
10. How do customer, product, promotion, and date dimensions affect sales performance?

---

## Dashboard Features

### 1. Product Performance Analysis

The product analysis page provides:

* Top 5 products by sales
* Bottom 5 products by sales
* Top 5 products by quantity sold
* Bottom 5 products by quantity sold
* Top 5 products by profit
* Bottom 5 products by profit

This allows stakeholders to quickly identify high-performing and underperforming products.

---

### 2. Period Comparison

The report provides interactive comparison between two user-selected date ranges.

Key metrics include:

* Total Sales
* Total Profit
* Total Units Sold

This enables users to compare business performance across different periods.

---

### 3. Sales Trend Analysis

The sales trends page provides:

* Sales over time
* Profit vs. Net Sales relationship
* Net Sales by City
* Total Orders
* Average Discount by Promotion

Interactive filtering allows users to explore specific products, customers, promotions, and dates.

---

### 4. Transaction-Level Analysis

A detailed transaction table allows users to drill down into individual records using filters such as:

* Date
* Customer
* Product
* Promotion

The table includes metrics such as:

* Customer ID
* Order ID
* Date
* Discount Percentage
* Discount Value
* Net Sales
* Price Per Unit
* Product ID
* Profit
* Promotion ID
* Total Sales
* Units Sold

This provides a detailed operational view beneath the executive-level dashboards.

---

## Data Model

The report uses a dimensional data model with a central fact table and supporting dimension tables.

### Fact Table

**Fact Table**

Contains transactional information including:

* Customer ID
* Product ID
* Promotion ID
* Date
* Sales
* Net Sales
* Discount
* Profit
* Units Sold

### Dimension Tables

**Dim Product**

* Product ID
* Product Name
* Product Line
* Price Per Unit

**Dim Customers**

* Customer ID
* Customer Name
* Email ID
* Phone Number
* City
* State
* Pincode

**Dim Promotion**

* Promotion ID
* Promotion Name
* Ad Type
* Coupon Code
* Percentage
* Price Reduction Type

**Date Tables**

Separate date tables are used to support independent date selections and period comparisons.

### Model Structure

```text
                 Dim Product
                     |
                     |
Dim Promotion → Fact Table ← Dim Customers
                     |
                     |
                 Date Table
```

A dedicated **Measures Table** is also used to organize DAX measures separately from the underlying data tables.

---

## Key Measures

The report uses DAX measures for important business KPIs, including:

* Total Sales
* Total Profit
* Total Units Sold
* Net Sales
* Sum of Discount
* Order Count
* Average Discount

These measures allow the dashboard to dynamically respond to slicers and filters.

---

## Tools & Technologies

| Tool                      | Purpose                                 |
| ------------------------- | --------------------------------------- |
| **Power BI**              | Dashboard development and visualization |
| **Power Query**           | Data cleaning and transformation        |
| **DAX**                   | Measures and business calculations      |
| **Data Modeling**         | Relationships and dimensional modeling  |
| **Microsoft Excel / CSV** | Source transactional data               |

---

## Data Preparation

The data preparation workflow included:

1. Importing raw transactional and dimension data
2. Inspecting data types and column structures
3. Cleaning and transforming source data using Power Query
4. Creating relationships between fact and dimension tables
5. Creating dedicated date tables
6. Building DAX measures for KPIs
7. Validating calculations against the underlying data
8. Designing interactive dashboards
9. Adding slicers and filtering capabilities
10. Testing the report from both summary and transaction-level perspectives

---

## Key Insights

Some of the major observations from the analysis include:

* **Apple iPhone 14** is the highest-performing product by sales and also ranks first in units sold.
* High-value consumer electronics contribute significantly to overall sales revenue.
* Some products generate relatively high unit volumes while contributing substantially less revenue due to lower selling prices.
* **Tupperware Lunch Box** appears among the lowest-performing products by revenue despite ranking relatively high in unit volume.
* Promotion performance varies considerably, with some promotions associated with substantially higher discount values.
* Sales demonstrate considerable variation over time, with several significant revenue spikes.
* Sales and profit show a strong positive relationship in the analyzed dataset.
* Geographic analysis indicates that sales are distributed across multiple cities rather than being concentrated in a single location.

> **Note:** These observations are based on the current dataset and dashboard configuration and are intended for analytical demonstration.

---

## How to Use

1. Download or clone this repository.
2. Open the `.pbix` file using **Microsoft Power BI Desktop**.
3. If required, update the data source paths.
4. Refresh the dataset.
5. Use the slicers and filters to explore the report.
6. Navigate between report pages to analyze product, sales, promotion, geographic, and transaction-level performance.

---

## Skills Demonstrated

This project demonstrates practical experience with:

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* Data Modeling
* Star Schema Concepts
* KPI Development
* Interactive Dashboard Design
* Time-Series Analysis
* Product Analysis
* Sales Analysis
* Profitability Analysis
* Promotion Analysis
* Geographic Analysis
* Transaction-Level Analysis
* Business Intelligence Reporting

---

## Project Outcome

The final report converts raw retail transaction data into an interactive analytical solution that can be used to monitor business performance, identify high- and low-performing products, compare sales periods, evaluate promotions, and investigate detailed transactions.

The project demonstrates an end-to-end workflow from **raw data → transformation → data modeling → DAX → visualization → business insights**.

---

## Author

**Siddharth Kar**

B.Tech | Data Analytics & Business Intelligence

**Tools:** Power BI · Excel · SQL · Python

---
