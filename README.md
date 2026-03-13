# Call-Center-Effectiveness---PowerBI-Dashboard

## Overview
This is an interactive and dynamic Power BI dashboard that  empowers the Company to track and enhance its customer satisfaction and employee performance. The aim is also to use real time visualizations to uncover hidden issues enabling training and process improvements ultimately to reduce costs, improve effectiveness and boost customer experience.

Dataset Source:
Kaggle — Call-Center-Dataset

---

## Objective

Build a single-page interactive dashboard that answers:
* How effectively is the call center handling incoming calls?
* Which agents are handling the highest number of calls and how does their performance compare to others?
* How quickly are customer calls being answered?
* Which types of customer issues generate the most calls and how successfully are they being resolved?
* Is the call center meeting its customer satisfaction targets?

---

## Dataset Audit

The dataset had 5001 rows and 10 columns (Call Id, Agent, Date, Time, Topic, Call Answered (Y/N), Problem 
Resolved(Y/N), Speed of answer in seconds, Talk Duration and Satisfaction rating). After thoroughly 
going through the dataset there was no evidence of NaN values, Null values and duplicated rows 
therefore all 5000 rows were used in the visualization.

---

## Data Cleaning and Transformation

Since the raw dataset had vague details, the following transformations were done using PowerBI:
* New Calculations were created for ‘% of calls answered and not answered’
* New Calculations were created for ‘Total Calls answered and not answered’
* New Measure was created for ‘If call was answered or not’ with binary values.
* New Measure was created for ‘If problem was resolved or not’ with binary values.
* New Measure was created to set the Maximum Satisfaction Value to 5 and Target Satisfaction was set to 4.50

---

## Data Model Logic
A dynamic selector controls the dashboard state:

* No selection → Overall view
* Topic selected → Problem Analysis
* Month selected → Productivity analysis
* Agent Selected → Performance analysis

---

## KPI's
* Total Calls
* Total Calls Answered
* Total Calls Resolved
* Average Speed of Answer
* Calls Answered by Agent
* Call Resolution Rate
* Calls Not Answered Rate
* Customer Satisfaction Score (CSAT)
* Satisfaction vs Target Satisfaction
* Call Volume by Day/Month
* Calls by Topic (Issue Category)
* Resolution Rate by Topic

---

## Visualisations

### 1. KPI Cards (Upper Row)
These give an overview into total calls, answered, resolved, best￾performing rep, and average answer time. 

### 2. Bar chart (Calls per Agent)
It indicates total answered and unanswered calls for each agent.It detects workload and responsiveness deficits.

### 3. Scatter Plot (Satisfaction vs. Answered Calls)
It brings together quality and quantity. It tells  you if agents who handle lots of calls are experiencing high satisfaction. This graph allows  you to balance service quality and performance

### 4. Line chart (day by day calls)
This chart plots the volume by date of each month showing daily and monthly trends.

### 5. Stacked Bar Graph (Resolved vs. Not Resolved by Topic)
The bar shows problem areas by topic of the calls and supports resource planning and training focus

## Key Insight
The call center is handling a high volume of calls, but customer satisfaction (3.40) is below the target (4.00), indicating a need to improve service quality or resolution effectiveness.

---

## How to Use

1. Select topic / month from slicer
2. Observe KPI changes
3. Analyze Performance Visuals
4. Use charts to identify best recommendation scenario

---

## Tools Used

* Power BI
* Data Modeling
