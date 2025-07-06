---
title: "Toy Products & Store Analytics – Toy Retail Sector"
excerpt: "Processed and visualized sales, profit, and inventory data of a multi-store toy business in Mexico to uncover product trends, pricing strategies, and stock inefficiencies using Python and Power BI.<br/><img src='/images/ToySales_Dashboard.jpg'  style='width: 51%; height: auto;  margin-top: 10px;'/>"
collection: portfolio
---


<img src='/images/ToySales_Dashboard.jpg'>


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
- Handled nulls and type mismatches, particularly in Date columns
- Corrected the **Date column's datatype** for proper time-based analysis

### Insights:

<img src="/images/ToySales_Table.jpg" width="500px">

- Products with Profit Margin > 25% are marked as **"High" Profit Status, else "Low"**
- **Lego Bricks, Magic Sand, Animal figure** need attention — they have **high costs but low returns**
- **Colorbuds and Action Figure** show excellent performance — **high profit and high margin.**
- Helps identify which products are cost-effective and which ones are draining profit.

---- 

<img src="/images/ToySales_KKPPI.jpg" width="500px">

- 1M Units Sold
- 14.44M in Sales
- 30K Units in Stock
- 10.43M in Total Cost
- 27.79% Profit Margin
- 4.01M in Profit

---

<p align="center">
  <img src="/images/LondonBike_outlier - Before.jpg" width="350px" style="display: inline-block;">
  <img src="/images/LondonBike_outlier - After.jpg" width="350px" style="display: inline-block;">
</p>

- Added 2 slicers to filter by **date (year/quarter) and store name.**