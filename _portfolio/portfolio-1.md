---
title: "London Bike Dataset Project"
excerpt: "How can data analytics on London’s bike-sharing system inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies ?<br/><img src='/images/500x300.png'>"
collection: portfolio
---

# London Bike Analytics

## Background :
As cities increasingly focus on sustainable urban transportation, it's essential to grasp the factors that shape public bike-sharing systems. This project delves into how environmental elements like weather, humidity, and wind, along with temporal aspects such as the season, time of day, weekdays versus weekends, and holidays, influence bike usage patterns in London.

The goal is to provide valuable insights that can inform inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies.

## : Dataset
- Over 17,00+ Entries
- 11 Features : date, time, Count of bike shares, real temp, temperature feels like, humidity, wind_speed, weather_code, is_holiday, is_weekend, season

## Tech Stack Used :
Python (Pandas, Numpy, Matplotlib, Seaborn), Tableau, Jupyter Notebook


## 🔍 Data Cleaning & Processing Steps

1. **Initial Inspection**
   - Loaded data with Pandas
   - Displayed data types, head, tail, and summary stats

2. **Datetime Handling**
   - Converted `timestamp` to `datetime`
   - Created `year`, `month`, `day`, and `weekday` columns

3. **Missing Values**
   - Checked and verified presence/absence of `NaN`s

4. **Data Type Conversion**
   - Ensured proper types for numerical and categorical columns

5. **Outlier Detection**
   - Used boxplots and statistical thresholds, IQR (Interquartile Range) to identify outliers

6. **EDA (Exploratory Data Analysis)**
   - Visualized trends over time
   - Plotted correlations between temperature, humidity, and bike usage

   