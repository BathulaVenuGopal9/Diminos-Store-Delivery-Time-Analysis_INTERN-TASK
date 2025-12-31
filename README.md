# Diminos-Store-Delivery-Time-Analysis_INTERN-TASK

## Project Overview

This project analyzes pizza delivery time performance for a Diminos franchise store.
The analysis focuses on evaluating Service Level Agreement (SLA) compliance using the 95th percentile of delivery time, a key metric used by Diminos to assess store performance.

The project demonstrates how data science can be applied to real-world business operations to prevent revenue loss and improve service efficiency.

## Business Problem

Diminos promises pizza delivery within 31 minutes.
If delivery exceeds this time, the order is provided free of cost.

Diminos evaluates store performance based on the following rule:

95th Percentile of Delivery Time < 31 minutes

Failure to meet this metric can result in loss of franchise ownership.

## Dataset Description

order_id – Unique order identifier

order_placed_at – Timestamp when the order was placed

order_delivered_at – Timestamp when the order was delivered

Each row represents a single pizza order.

## Feature Engineering

The dataset does not directly provide delivery duration.
Therefore, delivery time was derived as:

Delivery Time (minutes) = order_delivered_at − order_placed_at


This step enabled SLA and percentile-based evaluation.

## Analysis Approach

Data validation and timestamp conversion

Delivery time calculation in minutes

Distribution analysis of delivery times

95th percentile computation

SLA compliance assessment

Identification of extreme delays impacting performance

## Key Findings

Majority of orders are delivered within the promised time

A small number of extreme delays significantly impact the 95th percentile

Reducing outlier delays can immediately improve SLA compliance

## Business Recommendations

Introduce internal SLA buffers (target < 28 minutes)

Monitor real-time alerts for orders approaching delay thresholds

Optimize delivery staffing during peak hours

Focus on preventing extreme delivery delays rather than average performance

## Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn

Jupyter Notebook

# Conclusion

This project highlights the importance of percentile-based metrics in business decision-making and shows how targeted improvements in operational delays can significantly enhance SLA compliance and business sustainability.

# Author
Bathula Venu Gopal
Data Science Intern – Innomatics Research Labs
Batch 419
