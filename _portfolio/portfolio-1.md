---
title: "Operational Insights from London’s Bike Sharing Data"
excerpt: "How can data analytics on London’s bike-sharing system inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies ? <br/><img src='/images/London_cover.png' margin-top: 10px;'/>"
collection: portfolio
---

## [Github](https://github.com/mlaryan/London-Bike-Sharing-Dataset)  |  [Tableau](https://public.tableau.com/app/profile/aryan.dhanawade7402/viz/LondonBikeShareAnalytics/D1)

### Background :
As cities increasingly focus on sustainable urban transportation, it's essential to grasp the factors that shape public bike-sharing systems. This project delves into how environmental elements like weather, humidity, and wind, along with temporal aspects such as the season, time of day, weekdays versus weekends, and holidays, influence bike usage patterns in London.

The goal is to provide valuable insights that can inform inform business decisions regarding maintenance schedules, demand-based pricing, and promotional strategies.

### Business Use Cases / Applications :
- Time-specific promotions (“Weekend Ride Discount” or “Summer Pass Offers”)
- Workforce planning, Maintenance & redistribution
- Urban planning, Better station placement
- Demand-Based Pricing (pricing strategies based on time, weather, and holiday patterns)
- Identify periods of low usage (perform maintenance with minimal disruption to users)

---

### Dataset
- Over 17,000+ Entries
- 11 Features : date, time, Count of bike shares, real temp, temperature feels like, humidity, wind_speed, weather_code, is_holiday, is_weekend, season

---

### Tech Stack Used :
Python (Pandas, Numpy, Matplotlib, Seaborn), Tableau, Jupyter Notebook

---

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

5. **Outlier Detection**   [view data cleaning procedure.](https://github.com/mlaryan/London-Bike-Sharing-Dataset/blob/main/Data%20Cleaning%20and%20EDA.ipynb)
<p align="center">
  <img src="/images/LondonBike_outlier - Before.jpg" width="350px" style="display: inline-block;">
  <img src="/images/LondonBike_outlier - After.jpg" width="350px" style="display: inline-block;">
</p>

   - Used boxplots and statistical thresholds, IQR (Interquartile Range) to identify outliers

6. **EDA (Exploratory Data Analysis)**
   - Visualized trends over time
   - Plotted correlations between temperature, humidity, and bike usage.

---

### Data Visualization and outcome [Tableau](https://public.tableau.com/app/profile/aryan.dhanawade7402/viz/LondonBikeShareAnalytics/D1)

<img src="/images/KPI.jpg" width="300px">

- Grand total of all bike shares: **19,868,292**

---

<img src="/images/LondonBike_Each month count.jpg" width="500px">

- Total bike shares per month, aggregated over all years. 💡 Helps answer business questions like: "In which months should we increase bike availability or maintenance workforce ?"

---

<img src='/images/LondonBike_HourlyUsageTrends.jpg' width="800px">

- Peak Hours : Usage significantly **increases around 7:00 AM (1.6M shares) and again at 8:00 AM (2 shares)**, indicating a strong morning commute pattern. In the evening, usage at **5 PM (2M shares) and 6 PM (1.9M shares) is very high**, suggesting another peak. 

- Lunch time consistency : **Between 1 pm to 3 pm usage remains consistent around ~ 1 million**,💡 By identifying peak and off-peak hours, we can ensure bikes are available when demand is highest

- Consistency in Morning Troughs : **Between 1:00 AM and 4:00 AM, the usage hits very low points (around 100K shares)**, 💡 schedule maintenance during low-traffic periods (like 1 AM to 4 AM) to minimize service disruption.

---

<img src='/images/LondonBikeUserNumbs.jpg' width="500px" height="400px">

- Dominant Usage in Clear Weather: **Clear weather consistently shows the highest bike** usage by a significant margin in both 2015 and 2016, **followed by Scattered Clouds**. More clear-weather days = more demand.

- Impact of Rain/Cloudiness: **Light Rain Shower and Cloudy conditions have the lowest usage figures**. 💡 Targeted campaigns can be run to encourage rides during "less favorable but still manageable" weather

- Growth from 2015 to 2016: In most weather categories, there was an increase in bike usage from 2015 to 2016. The most **significant growth was seen in Cloudy conditions** (from 402,889 to 522,724).

---

<img src='/images/LondBike_Humidity & Wind Speed.jpg' width="800px">

- **As humidity increases, the average bike count decreases significantly** At 40% humidity → Avg. count ≈ 1,944; At 100% humidity → Avg. count ≈ 726

💡 Higher humidity is often associated with physical discomfort. leads to lower rider engagement - Sending weather-based alerts or discounts to encourage usage on humid days.

- **Bike usage drops significantly at higher wind speeds.** Peak usage around 20 km/h → Avg. count ≈ 1,361; Drops to 483 at 50 km/h wind speed. 💡 Apps can advise riders about expected wind conditions.

---

<img src='/images/London_Weekend-weekday.png.jpg' width="800px">

- Following chart suggests that the service is primiraly primarily used for daily commuting (e.g., work or school) rather than for leisure purposes. Resulting highest usage on weekdays. 💡 Holiday-specific promotions could help boost ridership on days when usage drop. 

----

### Conclusion :
-  Key operational insight suggests, clearly that bike usage is **heavily influenced by temporal and environmental factors** - with peak activity during weekday commute hours and under clear weather conditions.
- Commuting Behavior: Consistent peaks at 7–9 AM and 5–6 PM reaffirm the role in work-related travel, fortifying the **need for optimal bike availability during these windows.**
- Low-usage periods (1–4 AM) present **ideal windows for maintenance with minimal disruption.**
- Launch **targeted promotions for weekends & holidays** to boost leisure usage.
- Can **implement demand based pricing** and rebalancing course of action tied to time-of-day and weather forecasts.

