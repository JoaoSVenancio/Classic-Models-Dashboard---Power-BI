# Classic Models Dashboard - Power BI

## Overview

This repository contains the files and information necessary to recreate a comprehensive dashboard on "Classic Models" using Power BI. The dashboard provides insights into sales data, product lines, customer countries, and net profit analysis. The data is sourced from a MySQL database, and the process involves schema creation, data loading, and visualization creation in Power BI.

## Table of Contents

- [Data Preparation](#data-preparation)
- [MySQL Schema and Data Loading](#mysql-schema-and-data-loading)
- [Power BI Visualization](#power-bi-visualization)
  - [Page 1: Sales Analysis](#page-1-sales-analysis)
  - [Page 2: Net Profit Analysis](#page-2-net-profit-analysis)
- [Getting Started](#getting-started)

## Data Preparation

To create the "Classic Models" dashboard, a MySQL database was utilized. The dataset includes essential information such as order date, order number, product details, customer details, and sales-related metrics. The focus is on sales value, cost of sales, and their distribution across product lines, customer countries, and offices.

## MySQL Schema and Data Loading

1. **Script_Classic_Models.sql:** This file contains the SQL script for creating the necessary schema and loading the dataset into MySQL.

2. **View_PowerBI.sql:** In this file, you'll find the SQL script to create a view specifically designed for Power BI, including "sales value" and "cost of sales," with additional product and customer-level details.

## Power BI Visualization

### Page 1: Sales Analysis

- **Product and Year Filters:**
  - Two filters on the left-hand side allow users to choose specific products and years for focused analysis.

- **Clustered Bar Chart:** Illustrates Sales by Product Line.
- **Scatter Chart:** Represents Sales by Cost of Sales.
- **Donut Chart:** Displays Sales by Office.
- **Stacked Column Chart:** Depicts Sales by Customer Country.
- **Right Panel Metrics:**
  - Total Sales
  - Count of Unique Orders
  - Average Value of Each Order

### Page 2: Net Profit Analysis

- **Decomposition Tree:** Analyzes Net Profit explained by Customer Country, Product Line, and Customer Name.
- **Table:** Provides a Sales Overview with Year, Month, Sales Value, Sales Value MoM%, and Sales Value YTD.

## Getting Started

1. Clone this repository to your local machine.
2. Import the MySQL database using the provided schema and dataset by executing the scripts in `Script_Classic_Models.sql` and `View_PowerBI.sql`.
3. Open the Power BI file (`Classic Models Analysis.pbix`) to explore and visualize the "Classic Models" dashboard.

Feel free to customize and enhance the dashboard based on your specific requirements 🚀
