---
title: "Product & Store Analytics – Toy Retail Sector"
excerpt: "Processed and visualized sales, profit, and inventory data of a multi-store toy business in Mexico to uncover product trends, pricing strategies, and stock inefficiencies using Python and Power BI.<br/><img src='/images/ToySales_Dashboard.jpg'  style='width: 51%; height: auto;  margin-top: 10px;'/>"
collection: portfolio
---

### Background:

A toy business operating across multiple stores in Mexico and offering a variety of toy products is looking to gain a clearer picture of its **product sales**, **profitability**, and **inventory usage** across all store locations.

This project analyzes performance across **multiple stores**, **product categories**, and **time periods**, to uncover key insights.

### Business Use Cases / Applications:

To understand:
- Sales and profit trends across different products and stores
- Inventory inefficiencies (e.g: high stock but low sales)
- Products with high profit margins but low sales volume
- Best-performing product categories by store and over time
- Ideas for optimizing pricing based on performance trends

### Dataset:

<img src='/images/ToySales_DataModeling.jpg' width="800px">

### Tech Stack Used:

Python (Pandas, Numpy, Matplotlib, Seaborn), Power BI, Jupyter Notebook

### 🔍 Data Cleaning & Processing Steps:

- Imported the dataset using **Pandas**
- Used `.info()`, `.describe()`, and `.isnull().sum()` to understand the structure, data types, and missing values
- Detected some **outliers** in the data (through visualization) — but chose to **retain them** as they might reflect real-world business cases or exceptional events
- Corrected the **Date column's datatype** for proper time-based analysis

### Insights: