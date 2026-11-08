# User Habit and Marketing Strategy Case Study on a Bike-sharing System

## Project Overview
This project analyzes the behavioral discrepancies between **subscribed members** and **casual customers** using historical biking trip data. The ultimate goal is to formulate a set of targeted digital marketing strategies to convert casual riders into annual subscribers.

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
This phenomenon is likely due to users failing to lock or return bikes properly. To enhance data efficiency, I controlled valid trips to **1 to 60 minutes**. 
## Behavioral Analysis
<p align="center">
  <img src="<img width="978" height="796" alt="image" src="https://github.com/user-attachments/assets/c5b2b002-3306-4518-956f-0b60a35f25d6" />
</p>

### Key Observations
- **Contrast between frequency and duration**:
From the 1. trip duration chart, it is noticeable that casual users tend to rent the bikes for longer duration than members. However, the 2. weekly average chart demonstrates that members actually rents bikes more frequently than casual users. While casual users are inclined to rent bikes on weekends, members show a more steady renting duration across the entire week.
- **As a way of commuting**:
The 3. hourly trend chart clearly demonstrates that daily rental peaks occur at 7 AM and 5 PM. These periods directly correspond to corporate clock-in and clock-out hours, proving that bikes serve as a primary mode of transit during weekdays.
### Hypothesis
- **Not a habit**:
The inherent reason why casual users do not opt for subscription suggests that little frequency on using bikes; in other words, casual users do not cultivate a habit on using bikes as a way of commute in daily lives. It could be that traveling on bikes for their commute distance is just not cost-effective. Instead, **it is only a good deal when bikes can be used  during leisure activities on weekends.**
## Strategies
Based on the behavioral insights extracted above, the marketing strategy should focus on two aspects: **In-App Conversion** and **Location Targeting**.

### 1. APP Gamification on Weekends
As observed, casual riders dominate weekend usage, implying that users open the renting app more significantly during Saturdays and Sundays.
- **Action**: Launch a **"Weekend Lucky Draw"** gamification campaign during peak weekend hours. (11 a.m. - 4 p.m., as shown in 4. weekend hourly trend chart)
- **Incentive:** The lottery will distribute coupons on subscription fee, reducing conversion friction and lower the financial barrier for casual riders.

### 2. Targeting Location 
<img width="988" height="484" alt="image" src="https://github.com/user-attachments/assets/a15c40c6-291f-4f15-a894-8c1eadab0410" />

- **Action**: Launch weekday discount coupons at the top 5 weekend biking hotspots to provide a strong incentive for casual riders to rent during the week.
- **Incentive**: This strategy encourages casual users to experience the convenience of weekday biking, fostering a new daily routine and ultimately retaining them as permanent annual subscribers.
