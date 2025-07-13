---
title: "Credit Card Data : Exploratory Data Analysis using Python"
excerpt: "Performing an in-depth exploratory data analysis (EDA) of a credit card customer dataset using Python. The goal is to uncover meaningful patterns, demographic trends, behavioral insights, and potential business opportunities to aid in customer profiling, segmentation, and financial decision-making.<br/><img src='/images/500x300.png'>"
collection: portfolio
---

## [Github](https://github.com/mlaryan/In-depth-EDA-of-a-credit-card-customer-dataset)

---

### Background:
To perform an in-depth exploratory data analysis (EDA) of a credit card customer dataset using Python. The goal is to uncover meaningful patterns, demographic trends, behavioral insights, and potential business opportunities to aid in customer profiling, segmentation, and financial decision-making.


###  Dataset Overview:
- Source: Public dataset from Kaggle
- Nature: Tabular customer-level credit data and customer dataset
- Records: Includes features like demographic information, credit behavior, and financial indicators

- 🧾 Customer Dataset Key Columns:
Client_Num, Customer_Age, Gender, Dependent_Count, Education_Level,
Marital_Status, state_cd, Zipcode, Car_Owner, House_Owner,
Personal_loan, contact, Customer_Job, Income, Cust_Satisfaction_Score

- 🧾 Credit Card Dataset Key Columns:
Card_Category, Annual_Fees, Customer_Acq_Cost, Week_Start_Date, Week_Num, Qtr, current_year, 
Credit_Limit, Total_Revolving_Bal, Total_Trans_Amt, Total_Trans_Vol, Avg_Utilization_Ratio, 
Use Chip, Exp Type, Interest_Earned, Delinquent_Acc, Date, Month, Day, Month_Name


###  Tools & Technologies Used:
- Language: Python
- Libraries: pandas, matplotlib, seaborn, numpy


###  Insights from Customer Dataset:

<img src='/images/CreditCard_Histogram.png' width="600px">

- Age Distribution is Bell-Shaped: **centered around ages 45–50.** 
- Females (F) have a slightly higher peak than males in the 45–50 age range. 
- Very **few customers are below 30 or above 65**
- Very few customers are **below 30 or above 65**, indicating the bank’s primary customer base is likely employed, middle-aged adults

---

<img src='/images/CreditCard_Scatterplot.png' width="600px">

- A large number of customers earn below 100,000, forming a dense vertical block.
- Few customers appear **with very high income (>200K)**, but they are rare.
- Income appears evenly **spread across age groups up to 60**

---

<img src='/images/CreditCard_Insights.png' width="800px">

- Most customers are female, married, and self-employed.

---

<img src='/images/CreditCard_Barplotdoublt.png' width="600px">

- Majority of customers rated satisfaction as 3; Satisfaction scores **4 and 5 are reasonably common**
- Distribution is almost symmetrical, but slightly skewed towards higher satisfaction.

---

<img src='/images/CreditCard_PersonalLoan.png' width="600px">

- Females take slightly more personal loans than males.
- raduates take the most loans; postgraduates and doctorates the least.
- Married people take more loans than singles.
- Businessmen and self-employed take the most loans; retirees the least.

----

<img src='/images/CreditCard_CarOwners.png' width="600px">

- More females own cars than males.
- Graduates are the most likely to own cars.
- Married individuals are more likely to own cars than singles.
- Self-employed and businessmen show higher car ownership; blue-collar and retirees the least.

---

<img src='/images/CreditCard_Houseowners.png' width="600px">

- More females than males own houses.
- Graduates are the most likely to own houses.
- Married people show slightly higher house ownership.
- Self-employed and businessmen own more houses compared to other job types.

-----

