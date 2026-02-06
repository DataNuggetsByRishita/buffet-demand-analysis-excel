Buffet Demand Analysis (Excel Project)
Project Overview

This project analyzes buffet demand for a fine-dining restaurant located in a corporate area.
The restaurant experimented with offering buffet service across all days for three months but faced uncertainty around:

Which days should buffet be offered?

How much food should be prepared for buffet days to avoid waste or shortage?

Using transaction-level data and Excel-based analytics, this project converts raw sales data into actionable operational decisions.

Business Problem

The restaurant struggled with:

Inconsistent buffet demand across weekdays

High food wastage on low-demand days

No clear data-driven rule to decide buffet days

The goal was to identify optimal buffet days and estimate food preparation quantities using historical data.

Dataset Description

The dataset contains approximately 2,000 sales transactions with the following key attributes:

Transaction Date

Day of Week

Service Window (Lunch / Dinner)

Sale Type (Buffet / À La Carte)

Customer Count

Total Bill Amount

Tools & Techniques Used

Microsoft Excel

Pivot Tables

Conditional Logic (IF statements)

Feature Engineering

Descriptive & Decision-Focused Analytics

Analysis Approach
1️Data Preparation

Cleaned and structured transaction-level data

Created derived columns such as:

Buffet_Flag

Day_Number

Is_Lunch

Is_Weekend

2️Daily Demand Aggregation

Aggregated data to day + service window level

Calculated:

Total Customers per day

Buffet Probability (average of buffet selection)

This step reduced noise and revealed true demand patterns.

3️Buffet Probability Analysis

Buffet probability was calculated as:

Average of Buffet_Flag

This represents how likely customers choose buffet on a given day.

Key Observation:

Buffet demand was concentrated on Wednesday, Thursday, and Friday (Lunch)

Monday and Tuesday showed near-zero buffet preference

4️Decision Logic

A rule-based decision model was applied:

If Buffet_Probability ≥ 60% → Offer Buffet

Else → À La Carte Only

5️Food Preparation Planning

For buffet days:

Food prepared = Expected Customers × 1.3

For non-buffet days:

Food prepared = 0 (À La Carte service)

This ensures buffer stock while minimizing waste.

Key Insights

Buffet should only be offered on Wednesday, Thursday, and Friday (Lunch)

Monday, Tuesday, Saturday, and Sunday are not suitable for buffet

Dinner service showed negligible buffet demand

Controlled food preparation significantly reduces wastage

Business Impact

Data-driven buffet scheduling

Reduced operational costs

Clear daily food preparation guidelines

Scalable framework for future forecasting

Project Structure

Sales_Transactions – Raw data

Revenue_Analysis_By_Day_Service – Revenue patterns

Daily_Demand – Aggregated demand analysis

Daily_Demand_Table – Model-ready dataset

Decision & Food Planning – Final recommendations

Future Enhancements

Time-series forecasting

Regression-based demand prediction

Cost-profit optimization model

Automation using Python / Power BI

Author

Rishita
Aspiring Data Analyst | Business Analytics
Focused on practical, decision-oriented analytics projects
