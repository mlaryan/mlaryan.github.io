---
title: "Credit Card Data : Exploratory Data Analysis using Python"
excerpt: "Performing an in-depth exploratory data analysis (EDA) of a credit card customer dataset using Python. The goal is to uncover meaningful patterns, demographic trends, behavioral insights, and potential business opportunities to aid in customer profiling, segmentation, and financial decision-making.<br/><img src='/images/CreditCardCover.png' style='margin-top: 10px;'/>"
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

<p align="center">
  <img src="/images/CreditCard_Customer.png" width="350px" style="display: inline-block;">
  <img src="/images/CreditCard_Credit.png" width="380px" style="display: inline-block;">
</p>


###  Tools & Technologies Used:
- Language: Python
- Libraries: pandas, matplotlib, seaborn, numpy

----

###  Insights from Credit Card Dataset:

 <img src='/images/CreditCard_CardType.png' width="600px">

- "Swipe" method is by far the most common transaction type,  **approximately 7,000 transactions**
- Blue: Overwhelming majority, **~9,000 cards.** Gold: Very rare, **<50 cards.**
- Bills: Most frequent, **~3,000 occurrences**. Entertainment & Fuel: Significant, **~2,000 and ~1,700 transactions**

---

<img src='/images/CreditCard_ScatterPlots.png' width="600px">

- Total Trans Amount vs Credit Limit : No strong linear correlation; transaction **amounts are spread across limits.**
- Total Trans Amount vs Total Trans Volume: As Total_Trans_Amount increases, **Total_Trans_Vol increases proportionally, showing some clustered steps.**
- Annual Fees vs Credit Limit: No clear linear correlation; **high credit limits can have low fees, and vice-versa.**

---

<img src='/images/CreditCard_LineSchart.png' width="600px">

- Customer_Acq_Cost: Peaks April-May (~100), lowest March/late year (~95), **showing seasonality.**
- Annual_Fees: **Highs in March-April (~305-310)**, lows in early/late year (~280-285).
- Credit_Limit: Highest July-Aug (>9500), lowest March-April/Sept-Oct (7500-8000); **increases mid-year.**
- Total_Trans_Amt: Peaks July (~4800), lowest April/Oct (4100-4200), **reflecting mid-year spending increase.**
- Total_Trans_Vol: Mirrors amount: peaks July (~67), **lowest March-April/Sept-Oct (~62.5-63).**
- Interest_Earned: Highest July-Aug (~875-880), lowest March-April/Oct-Nov (700-750), **spiking with mid-year activity.**


---

---


##  Insights from Customer Dataset:

<img src='/images/CreditCard_Histogram.png' width="600px">

- Age Distribution is Bell-Shaped: **centered around ages 45–50.** 
- Females (F) have a slightly higher peak than males in the 45–50 age range. 
- Very **few customers are below 30 or above 65**
- Very few customers are **below 30 or above 65**, indicating the bank’s primary customer base is likely employed, middle-aged adults

---

<img src='/images/CreditCard_Scatterplot.png' width="600px">

- A large number of customers earn below 120,000, **forming a dense vertical block.**
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

- Females take slightly **more personal loans than males.**
- Graduates take the most loans; postgraduates and doctorates the least.
- **Married people take more loans** than singles.
- Businessmen and self-employed take the most loans; retirees the least.

----

<img src='/images/CreditCard_CarOwners.png' width="600px">

- More females own cars than males.
- Graduates are the most likely to own cars.
- Married individuals are more likely to own cars than singles.
- Self-employed and businessmen show higher car ownership; blue-collar and retirees the least.

---

<img src='/images/CreditCard_Houseowners.png' width="700px">

- More females than males own houses.
- Graduates are the most likely to own houses.
- Married people show slightly higher house ownership.
- Self-employed and businessmen own more houses compared to other job types.

-----

