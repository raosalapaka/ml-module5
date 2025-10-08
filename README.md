# Overview

This READMe has the analysis for acceptance rates of two coupon types: Bar and CoffeeHouse. First the Bar coupon type is analyzed and then the CoffeeHouse. The Jupyter notebook assignment5_1_RS.ipynb has the code for this analysis

Link to the jupyter notebook: [Assignment 5_1 Jupyter notebook](https://github.com/raosalapaka/ml-module5/blob/main/assignment5_1_RS.ipynb)

Link to the repository: [Git repository](https://github.com/raosalapaka/ml-module5.git) 

# Analysis

---
# **Bar coupons acceptance rates**

## **Context**

This analysis focuses only on the Bar coupons. It tries to identify categories of drivers and other attributes that have an impact on the acceptance rates of the Bar coupons. For context, the number of Bar coupons is 1913 out of a total of 12079 coupons in total

The data was cleaned by dropping the car column as there wasn't significant data available. Also towards cleaning the data, we dropped the rows that had null values. This resulted in 4.7% of the rows being dropped. The assumption is that this is acceptable given there are 12079 remaining rows that should be enough to provide useful insights

## **Findings**

- Overall across all types of coupons, ~57% of the coupons were accepted
- Acceptance rates were slightly higher when the tempearture was greater than 80 degrees. One reason for this could be people went to bars more when the weather was good and sunny. The difference is not huge but noticeable (~60% against ~53%)
- Acceptance rate was almost double among those who went to bar 4 or more times than those who went to bar 3 or fewer times (76% vs 37%)

   <img width="465" height="287" alt="image" src="https://github.com/user-attachments/assets/cd82b308-f72a-43c4-b058-3160a87ef93d" />

-  Acceptance rates among those who went to bar at least once and who were 25 years or older was significantly higher than others (almost double - 69% vs 34%)

   <img width="465" height="287" alt="image" src="https://github.com/user-attachments/assets/7857dfa2-fb7d-4749-b37e-41ec67759a6e" />

-  Acceptance rates for those who went to bar at least once, the passengers who were adults (not kids) and whose occupation was not 'Farming, Fishing or Forestry' was signficantly higher than all others (more than double 70% vs 30%)

   <img width="465" height="287" alt="image" src="https://github.com/user-attachments/assets/db979d48-242c-45fb-b016-d985c24a9613" />

- Those who went to bar at least once a month, analysis of their age, marital status and income indicates that
   1. Rate of acceptance is much higher for those who are adults (not kids) and who are not widowed
   2. Rate of acceptance is much higher for those under 30 than all others
   3. There is not much of a difference based on income - acceptance rate was slightly higher for those who earned less than 50K

      
   <img width="842" height="407" alt="image" src="https://github.com/user-attachments/assets/efe40e5c-f885-4cd3-a408-638c20fda1a2" />

## **Conclusion**

Given the above findings, there is a greater likelihood that people in following cohorts will have higher acceptance rate:

- who went to bar at least 4 or more times a month
- who go to bar at least once a month and are 25 years of age or older
- who go to bar at least once a month and are adults and not working in 'Farming, Fishing or Forestry'
- who go to bar at least once a month and are not widowed and are over 30 years of age

Conversely, there is opportunity in focusing on the following cohorts to increase their accept rates:

- those who go to bars less than 3 times a month
- younger population especially people in the age group 20-30
  
---
# Coffee House coupons acceptance rates

## Context

This analysis focuses only on the _Coffee_ _House_ coupons. It tries to identify categories of drivers and other attributes that have an impact on the acceptance rates of the Coffee House coupons. For context, the number of Coffee House coupons is 3816 out of a total of 12079 coupons in total which is the highest amongst all types of coupons

The data was cleaned by dropping the car column as there wasn't significant data available. Also towards cleaning the data, we dropped the rows that had null values. This resulted in 4.7% of the rows being dropped. The assumption is that this is acceptable given there are 12079 remaining rows that should be enough to provide useful insights

## Findings

- Overall across all types of coupons, ~57% of the coupons were accepted
- Acceptance rate was much higher for those who went to Coffee House at least once than those who went there less than once a month (almost double, 66% vs 34%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/dc116963-4dbd-464e-bb62-b07d74d9c206" />

- Acceptance rate was significantly higher for those who went to the Coffee House at least once a month and were of age 26 or below (68% vs 43%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/cb5adc26-6e81-4406-ac17-39ec63993e34" />

- Acceptance rate was significantly higher for passengers who went to Coffee House at least once a month, had no urgent destination and were with friends or partners (77% vs 44%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/a4012c2a-aee7-4687-95c1-8956e420a4a3" />

- Acceptance rates based on gender (male/female) was not much different (64% vs 67%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/bff0a2f9-1cba-45d5-9f61-4bbeb6321781" />

- Acceptance rates were much higher between 10AM and 2PM for those who went to Coffee House at least once (77% vs 28% which is almost 2.5 times)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/e91a1020-03eb-439d-8d1e-6bd9ac7da7ad" />

- Acceptance rates were higher when whether was Sunny for those who went to the Coffee House at least once (67% vs 49%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/1e969872-2eca-4192-b339-bdd27d6c578f" />

- Acceptance rates higher for those who went to the Coffee House at least once with High School diplomas then all others including graduate degrees (72% vs 48%)

   <img width="462" height="289" alt="image" src="https://github.com/user-attachments/assets/1d801103-c60d-4224-b7e6-a97ad621bfcc" />

## Conclusion

Given above findings, there is a higher likelihood of Coffee House coupon being accepted by the following cohorts

- who  go to Coffee House at least once
- who are below 26 years of age
- who are with friends and have no urgent destination
- between 10AM and 2PM
- during Sunny weather and
- who have a high school diploma

Conversely, there is opportunity to increase acceptance rates for the following cohorts

- who are above 26 years of age
- who are not with friends or partners and are going to a fixed destination
- outside of 10AM and 2PM
- rainy weather and people with higher than high school diplomas

## Future work

- look also at different coupon types and see which coupons are more likely to be accepted
- the above analysis seems one dimensional - there is opportunity to look at different combinations of cohorts and see if there is some aspect that distinguishes in some way (w.r.t accept rate which could be very high or very low)
- there is an oppotunity to convert the columns to numeric and run pairplots to analyze relationships between different features of the data set
