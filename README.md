# Massachusetts General Hospital Analysis

## Table of Contents

## Introduction
In the modern healthcare landscape, understanding patient demographics, encounter types, and cost distributions is vital for improving operational efficiency and patient care outcomes. This project provides a comprehensive analysis of healthcare data from Massachusetts General Hospital using hospital records from year 2011 to 2022  to uncover patterns, and make insightful decisions.

## Project Description
The project covers data collection, cleaning, and structured analysis of hospital records. It involves processing multiple datasets including patient profiles, payer information, clinical encounters, and surgical procedures to address key business and healthcare questions.

## Business Questions
This analysis was guided by the following business questions;
- What is the re-admission rate per 30days? 
- Does insurance coverage affect re-admission rate and Length of stay durations 
within patients with similar diagnosis? 
- What demographic group is associated with longer/shorter stay duration and 
higher re-admission rate? 
- What procedure incurs the most cost post insurance coverage? 
- What department records the highest case of re-admissions? 
- What demographic and operational factors are most strongly associated with 
length of stay above the average for each department? 

## About the Dataset
The analysis is based on the **Massachusetts General Hospital Dataset**, consisting of several interconnected tables:
- **Patients:** Demographic data (ID, Birth Date, Gender, Race, Location).
- **Encounters:** Details on hospital visits (Start/Stop times, Encounter Class, Total Claim Cost, Payer ID).
- **Payers:** Information on insurance providers (Medicare, Medicaid, Dual Eligible, etc.).
- **Procedures:** Data on medical procedures performed and their associated costs.
- **Pivot Tables:** Aggregated views of re-admission distributions and costs per department.

## Tools Used
- **Microsoft Excel:** Used for initial data exploration, cleaning, and the creation of Pivot Tables and Charts.

## Methodology
- **Standardization:** Ensured "Gender" and "Race" fields followed a consistent naming convention.
- **Date Handling:** Converted Start/Stop times from onverted ISO 8601 format into standard Date/Time formats.
- **Missing Values:** Handled empty fields by labeling them appropriately('Unspecified,etc)
- **Integrity:** Verified that Patient IDs in the Encounters table matched the master Patient list.

## Data Modeling
Calculated fields were created to determine:
- **Length of Stay:** Difference between Stop and Start times.
- **Cost Post Payer Coverage:** The remaining balance after insurance contributions.
- **Re-admission Status:** Categorized based on follow-up encounter patterns.
- **Age:** Yearfraction between Birth date and Death date. 

## Data Analysis
Key metrics analyzed include:
- **Patient Volume:** Total count of unique patients.
- **Financials:** Total Claim Cost and Payer Coverage vs. Out-of-pocket costs.
- **Demographics:** Analysis of patient distribution by City (e.g., Boston, Quincy, Medford) and Gender.
- **Departmental Performance:** Encounter counts by class (Ambulatory, Emergency, Inpatient, Urgent Care, Wellness).

## Data Visualization
![Dashboard Overview](Overview.png)
![Uploading image.png…](https://github.com/ChimchetamIbeh/Massachusetts-General-Hospital-Analysis/blob/e7ebd8ae5a6b69cb4778d25be47131221857ad50/Operational%20Cost.png)
![Uploading image.png…](https://github.com/ChimchetamIbeh/Massachusetts-General-Hospital-Analysis/blob/e7ebd8ae5a6b69cb4778d25be47131221857ad50/Re-Admission%20and%20Length%20of%20Stay.png)
- **Re-admissions by Department:** A bar chart showing that Ambulatory and Urgent Care have the highest re-admission counts.
- **Total Cost per Department:** A breakdown of revenue generated across different hospital wings.
- **Payer Distribution:** A pie chart showing the share of claims handled by Medicare, Medicaid, and private payers.

## Key Insights
- **High Volume Departments:** Ambulatory services account for the largest portion of encounters (over 8,000 re-admissions).
- **Cost Drivers:** Inpatient and Urgent Care represent a significant portion of the total claim costs despite lower volumes compared to Ambulatory care.
- **Demographic Trends:** A significant portion of the patient base is concentrated in the Suffolk County/Boston area.

## Recommendations
- **Resource Allocation:** Increase staffing in Ambulatory and Urgent Care during peak periods identified in the time-series analysis.
- **Re-admission Strategy:** Investigate the high re-admission rates in the Ambulatory department to determine if post-discharge care protocols need adjustment.
- **Financial Optimization:** Review the "Cost Post Payer Coverage" to identify if certain demographics are facing higher out-of-pocket burdens.

## 13. Conclusion
The insights derived from the Massachusetts General Hospital dataset provide a roadmap for optimizing department-specific resources and improving patient throughput. By addressing re-admission trends, the hospital can enhance both patient satisfaction and financial stability.

## 14. Contact Information
- **LinkedIn:** [www.linkedin.com/in/ibeh-chimchetam]
- **Email:** [ibehchimchetam@gmail.com]
