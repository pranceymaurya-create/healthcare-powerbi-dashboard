# healthcare-powerbi-dashboard

1 – Title Slide

SMART HEALTHCARE ANALYTICS DASHBOARD

Course: Data Visualization & Business Intelligence with Power BI
Program: BCA – Silver Oak University

Student Name: Prancey Maurya

Project: Dynamic Healthcare Data Dashboard using Power BI

 2 – Problem Statement

Healthcare organizations generate a huge amount of patient and hospital data every day.

However:

Raw healthcare data is difficult to analyze manually.

Hospitals need insights about patients, billing, and medical conditions.

Decision making becomes slow without proper visualization tools.

Objective of the project

To build an interactive Power BI dashboard that helps analyze:

Patient statistics

Medical conditions

Hospital billing

Insurance data

Healthcare trends

This dashboard helps hospital management make better data-driven decisions.

3– Data Source

The dataset used is a Healthcare Dataset (CSV format).

The dataset includes the following fields:

Patient Information

Name

Age

Gender

Blood Type

Hospital Information

Hospital

Doctor

Room Number

Medical Information

Medical Condition

Medication

Test Results

Financial Information

Billing Amount

Insurance Provider

Admission Information

Admission Date

Discharge Date

Length of Stay

Data cleaning and transformation were performed using Power BI Power Query Editor.

 4 – Data Preparation (What I Did)

Before building the dashboard, the dataset was prepared.

Steps performed:

• Removed unnecessary columns
• Corrected data types
• Converted dates properly
• Handled missing values
• Created calculated columns
• Created DAX measures for KPIs

This ensured the dataset is clean, structured, and ready for visualization.

5 – Calculated Columns Used

Some calculated columns were created to improve analysis.

Examples:

Length of Stay

Length of Stay = DATEDIFF('healthcare_dataset'[Date of Admission],
'healthcare_dataset'[Discharge Date], DAY)

Billing Category

Billing Category =
IF('healthcare_dataset'[Billing Amount] > 30000,
"High Cost","Normal Cost")

These columns help analyze:

Patient stay duration

Treatment cost categories

 6 – DAX Measures Created

Several measures were created for KPIs and analysis.

Total Patients

Total Patients = COUNT('healthcare_dataset'[Name])

Total Charges

Total Charges = SUM('healthcare_dataset'[Billing Amount])

Average Age

Average Age = AVERAGE('healthcare_dataset'[Age])

Average Stay

Avg Stay = AVERAGE('healthcare_dataset'[Length of Stay])

Male Patients

Male Patients =
CALCULATE(COUNT('healthcare_dataset'[Name]),
'healthcare_dataset'[Gender] = "Male")

Female Patients

Female Patients =
CALCULATE(COUNT('healthcare_dataset'[Name]),
'healthcare_dataset'[Gender] = "Female")
7 – Dashboard Overview

The project includes 3 dashboard pages:

1️⃣ Smart Healthcare Analytics

Shows overall hospital statistics:

Total Patients

Total Charges

Average Age

Average Stay

Patient distribution by gender

Medical condition vs billing

2️⃣ Medical Insights

Focuses on medical analysis:

Blood type vs condition

Average stay by condition

Condition distribution

Cost category by condition

3️⃣ Financial Analytics

Focuses on hospital financial performance:

Charges by insurance provider

Charges by hospital

Doctor billing analysis

Stay vs billing relationship

8 – Dashboard Features

The dashboard includes several interactive features.

✔ KPI Cards
✔ Bar Charts
✔ Line Charts
✔ Pie & Donut Charts
✔ Tables
✔ Scatter Plots

Interactive Filters (Slicers):

Hospital

Gender

Blood Type

Insurance Provider

Medical Condition

Doctor

These allow users to filter and analyze the data dynamically.

9 – Page 1 (Smart Healthcare Analytics)

This page shows overall healthcare performance.

Main KPIs:

56K Total Patients

1.42 Billion Total Charges

15.5 Average Stay

51 Average Age

Visualizations include:

Total charges by year

Patient distribution by gender

Medical condition vs billing

This provides a quick overview of hospital operations.

10 – Page 2 (Medical Insights)

This page focuses on medical condition analysis.

Key visualizations:

• Blood Type vs Medical Condition table
• Average stay by condition
• Condition percentage distribution
• Cost category by condition

This helps hospitals understand:

Which diseases are common

How long patients stay

Which treatments are expensive

 11 – Page 3 (Financial Analytics)

This page analyzes financial performance.

Key visualizations:

• Total charges by insurance provider
• Charges by hospital
• Doctor-wise billing table
• Scatter chart for stay vs billing amount

This helps management understand:

Revenue sources

Insurance contribution

Hospital performance

12 – Key Insights

Important insights discovered from the dashboard:

• Total patients analyzed: 56,000+
• Total healthcare charges: 1.42 Billion
• Average patient age: 51 years
• Average hospital stay: 15.5 days

Medical findings:

Diabetes and hypertension are common conditions

Some conditions require longer hospital stays

Financial findings:

Insurance providers contribute major revenue

Some hospitals generate higher charges

13 – Conclusion

This project demonstrates how Power BI can transform raw healthcare data into meaningful insights.

Benefits of the dashboard:

✔ Better healthcare analysis
✔ Faster decision making
✔ Easy visualization of complex data
✔ Interactive exploration using filters

This dashboard helps hospitals improve patient care, cost management, and operational efficiency.

– Thank You
