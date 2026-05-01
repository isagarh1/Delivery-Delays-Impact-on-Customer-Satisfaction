# Delivery-Delays-Impact-on-Customer-Satisfaction
Analyzing how delivery delays impact customer satisfaction and identifying system-wide operational inefficiencies.


## Overview

This project analyzes how delivery performance affects customer satisfaction using an e-commerce dataset (~99K orders, ~R$13.6M revenue).

The goal is to identify whether delivery delays impact customer experience and determine where operational improvements should be focused.

## Business Problem

In e-commerce, delivery performance is a key driver of customer satisfaction.

This project answers:

- Do delivery delays reduce customer satisfaction?
- How significant is the impact?
- Are delays region-specific or system-wide?

## Dataset
- Source: Olist Brazilian E-commerce Dataset
- Records: ~99,000 orders
- Revenue: ~R$13.6M
## Key fields:
- Order dates (purchase, estimated delivery, actual delivery)
- Review scores (proxy for customer satisfaction)
- Customer location (state)

## Approach
Data Preparation
- Cleaned and transformed multiple tables (orders, customers, reviews, products)
- Created relationships using a star schema model
- Calculated delivery delay using:
- Estimated vs actual delivery dates
## Feature Engineering
Created Delivery Status categories:
- Early
- On Time
- Slight Delay
- Moderate Delay
- Severe Delay
## Built key measures:
- Total Revenue
- Total Orders
- Average Review Score
- Delayed Orders %
## Analysis
- Compared customer satisfaction across delivery categories
- Evaluated impact vs volume (review score + order count)
- Performed regional analysis using state-level data
- Tested correlation between delay % and satisfaction

## Key Insights
- 38% of orders are delayed, indicating a systemic operational issue  
- Customer satisfaction drops sharply even with minor delays:  
  - On-time: ~4.18  
  - Slight delay: ~3.29 (~20% decrease)  
- Moderate delays represent the **highest business risk**, combining high frequency with significant satisfaction drop  
- Severe delays have the lowest ratings but lower occurrence, making them less impactful overall  
- Minimal variation across states → delays are driven by **system-wide inefficiencies**, not regional issues
- 
## Business Recommendations
- Focus on reducing moderate delays, as they affect the most customers
- Identify and fix bottlenecks in the delivery process
- Provide more accurate delivery timelines to customers
- Improve overall delivery operations rather than targeting specific regions

 ## Dashboard Features
- KPI overview (Revenue, Orders, Review Score, Delay %)
- Delivery performance vs customer satisfaction analysis
- State-level delay analysis
- Interactive slicer (state filter)

## Tools Used
- Power BI
- DAX (Data Analysis Expressions)
- Data Modeling (Star Schema)
  
## Key Takeaway

Delivery delays have a significant negative impact on customer satisfaction, even at minor levels.
Since the issue is consistent across regions, improving overall delivery operations is more effective than localized fixes.

## Dashboard Preview
<img width="1323" height="762" alt="Delivery Delays Impact on Customer Satisfaction" src="https://github.com/user-attachments/assets/c3c388b2-1881-48eb-8569-d21fc630bd7b" />





