# User Habit and Marketing Strategy Case Study on a Bike-sharing System

## Project Overview
This project analyzes the behavioral discrepancies between **subscribed members** and **casual customers** using historical biking trip data. The ultimate goal is to identify formulate a set of targeted digital marketing strategies to convert casual riders into annual subscribers.

## Background & Pricing Structure
The system offers flexible mobility options with three pricing tiers: single-ride passes, full-day passes, and annual memberships. 
- **Casual Riders:** Users who purchase single-ride or full-day passes.
- **Annual Members:** Users with annual subscriptions. This segment represents the company's most profitable revenue stream.

## Data Infrastructure 
- **Data Scale:** Historical trip data from Jan. 2026 to Jun. 2026 (Google Coursera Data Analysis Capstone).
- **Data Infrastructure:** Google BigQuery (SQL)for data cleaning, table joins, and feature extraction.
- **Analysis & Visualization:** Python (Pandas, Seaborn, Matplotlib) for generating data graphs. 

## Data Cleaning 
Anomalies were detected in the riding duration metrics, where the 75th percentile (`Q3`) was merely **18.7 minutes**, yet the maximum value reached an unrealistic **1,499 minutes**. 
Such a phonemenon can due to users failing to lock or return bikes properly. To enhance data efficiency, I controlled valid trips to **1 to 60 minutes**. 
## Behavioral Analysis
<table border="0" width="100%">
  <tr>
    <td width="50%" align="center" valign="top">
      <p><b>1. Contrast in Riding Time</b></p>
      <img src="https://github.com/user-attachments/assets/a675ef9f-c041-4a17-896a-37cac7bbe30e" width="100%" /> 
    </td>
    <td width="50%" align="center" valign="top">
      <p><b>2. Daily Average Riding Volume</b></p>
      <img src="https://github.com/user-attachments/assets/8ea8b4d7-630e-4d35-816b-9f302a68115c" width="100%" />
    </td>
  </tr>
</table>

<table border="0" width="100%">
  <tr>
    <td width="50%" align="center" valign="top">
      <p><b>3.Daily Renting Peak</b></p>
   <img width="862" height="554" alt="image" src="https://github.com/user-attachments/assets/306eb34b-012a-4bc3-8be9-e3c4bcfd37d0" width="100%"/>
  </td>
  <td>
       <p><b>4. Weekend Hourly Trend</b></p>
  <img src="https://github.com/user-attachments/assets/de8f794b-9245-4ec7-b75c-22d94df2d84e" width="100%" />
</td>
  </tr>
</table>

### Key Observations
- **Contrast between frequency and duration**:
From the trip duration (1.) chart, it is noticeable that casual users tend to rent the bikes for longer duration than members. However, the weekly average (2.) chart demonstrates that members actually rents bikes more frequently than casual users. While casual users are inclined to rent bikes on weekends, members show a more steady renting duration across the entire week.
- **As a way of commuting**:
The hourly trend (3.) chart clearly demonstrates that daily rental peaks occur at 7 AM and 5 PM. These periods directly correspond to corporate clock-in and clock-out hours, proving that bikes serve as a primary mode of transit during weekdays.
### Hypothesis
- **Not a habit**:
The inherent reason why casual users do not opt for subscription could due to little frequency on using bikes; in other words, casual users do not cultivate a habit on using bikes as a way of commute in daily lives. It could be that traveling on bikes for their commute distance is just not cost-effective. Instead, **it is only a good deal when bikes can be used  during lesiure activities on weekends.**
## Strategies
Based on the behavioral insights extracted above, the marketing strategy should focus on two asepcts: **In-App Conversion** and **Location Targeting**.

### 1. APP Gamification on Weekends
As observed, casual riders dominate weekend usage, implying that users open the renting app more significantly during Saturdays and Sundays.
- **Action**: Launch a **"Weekend Lucky Draw"** gamification campaign during peak weekend hours. (11 a.m. - 4 p.m., as shown in 4. weekend hourly trend chart)
* **Incentive:** The lottery will distribute coupons on subscription fee, reducing conversion friction and lower the financial barrier for casual riders.

### 2. Targeting Location 
<img width="988" height="484" alt="image" src="https://github.com/user-attachments/assets/a15c40c6-291f-4f15-a894-8c1eadab0410" />

- **Action**: Launch weekday discount coupons at the top 5 weekend biking hotspots to provide a strong incentive for casual riders to rent during the week. This strategy encourages casual users to experience the convenience of weekday biking, fostering a new daily routine and ultimately retaining them as permanent annual subscribers.
