---
title: "London Bike Shares Analytics"
excerpt: "How can data analytics on London’s bike-sharing system inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies ? <br/><img src='/images/London_cover.png'>"
collection: portfolio
---

## [Github](https://github.com/mlaryan/London-Bike-Sharing-Dataset) [Tableau](https://public.tableau.com/app/profile/aryan.dhanawade7402/viz/LondonBikeShareAnalytics/D1)

### Background :
As cities increasingly focus on sustainable urban transportation, it's essential to grasp the factors that shape public bike-sharing systems. This project delves into how environmental elements like weather, humidity, and wind, along with temporal aspects such as the season, time of day, weekdays versus weekends, and holidays, influence bike usage patterns in London.

The goal is to provide valuable insights that can inform inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies.

### Business Use Cases / Applications :
- Time-specific promotions (“Weekend Ride Discount” or “Summer Pass Offers”)
- Workforce planning, Maintenance & redistribution
- Urban planning, Better station placement
- Demand-Based Pricing (pricing strategies based on time, weather, and holiday patterns)
- Identify periods of low usage (perform maintenance with minimal disruption to users)

### Dataset
- Over 17,00+ Entries
- 11 Features : date, time, Count of bike shares, real temp, temperature feels like, humidity, wind_speed, weather_code, is_holiday, is_weekend, season

### Tech Stack Used :
Python (Pandas, Numpy, Matplotlib, Seaborn), Tableau, Jupyter Notebook


### 🔍 Data Cleaning & Processing Steps [Github](https://github.com/mlaryan/London-Bike-Sharing-Dataset)

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
   - Plotted correlations between temperature, humidity, and bike usage.

### Data Visualization and outcome [Tableau](https://public.tableau.com/app/profile/aryan.dhanawade7402/viz/LondonBikeShareAnalytics/D1)

<img src='/images/London_cover.png' width="600px">

- Peak Hours : Usage significantly increases around 7:00 AM (1,66,309 shares) and then again at 8:00 AM (2,087,164 shares), indicating a strong morning commute pattern. In the evening, usage at 5 PM (2,059,938 shares) and 6 PM (1,913,944 shares) is very high, suggesting another peak.

- Lunch time consistency : Between 1 pm to 3 pm usage remains consistent aorund ~ 1 million

- Consistency in Morning Troughs :  Between 1:00 AM and 4:00 AM, the usage consistently hits very low points (around 100K shares or less), reinforcing the idea that these are indeed very low-demand hours.

