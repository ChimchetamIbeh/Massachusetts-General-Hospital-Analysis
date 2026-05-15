# Massachusetts General Hospital Analysis

## 1. Introduction
This project provides a comprehensive analysis of healthcare data from Massachusetts General Hospital. In the modern healthcare landscape, understanding patient demographics, encounter types, and cost distributions is vital for improving operational efficiency and patient care outcomes.

## 2. Project Description
The project covers data collection, cleaning, and structured analysis of hospital records. It involves processing multiple datasets including patient profiles, payer information, clinical encounters, and surgical procedures to address key business and healthcare questions.

## 3. Project Aim
The primary goal is to analyze patient and encounter data to identify healthcare trends, assess the financial impact of different encounter classes, and provide actionable recommendations for hospital administration regarding re-admission rates and cost management.

## 4. About the Dataset
The analysis is based on the **Massachusetts General Hospital Dataset**, consisting of several interconnected tables:
- **Patients:** Demographic data (ID, Birth Date, Gender, Race, Location).
- **Encounters:** Details on hospital visits (Start/Stop times, Encounter Class, Total Claim Cost, Payer ID).
- **Payers:** Information on insurance providers (Medicare, Medicaid, Dual Eligible, etc.).
- **Procedures:** Data on medical procedures performed and their associated costs.
- **Pivot Tables:** Aggregated views of re-admission distributions and costs per department.

## 5. Tools Used
- **Microsoft Excel:** Used for initial data exploration, cleaning, and the creation of Pivot Tables and Charts.
- **GitHub:** Used for project hosting and documentation.

## 6. Importing the Dataset
The dataset was originally provided in `csv` format. The sheets were imported into Excel, where the analysis took place.

## 7. Data Cleaning & Transformation
- **Standardization:** Ensured "Gender" and "Race" fields followed a consistent naming convention.
- **Date Handling:** Converted Start/Stop times into standard Date/Time formats to calculate "Length of Stay."
- **Missing Values:** Handled empty "Reason Code" fields by labeling them as "Unspecified."
- **Integrity:** Verified that Patient IDs in the Encounters table matched the master Patient list.

## 8. Data Modeling
Calculated fields were created to determine:
- **Length of Stay:** Difference between Stop and Start times.
- **Cost Post Payer Coverage:** The remaining balance after insurance contributions.
- **Re-admission Status:** Categorized based on follow-up encounter patterns.
- **Age:** Yearfraction between Birth date and Death date. 

## 9. Data Analysis
Key metrics analyzed include:
- **Patient Volume:** Total count of unique patients.
- **Financials:** Total Claim Cost and Payer Coverage vs. Out-of-pocket costs.
- **Demographics:** Analysis of patient distribution by City (e.g., Boston, Quincy, Medford) and Gender.
- **Departmental Performance:** Encounter counts by class (Ambulatory, Emergency, Inpatient, Urgent Care, Wellness).

## 10. Data Visualization
![Dashboard Overview]()
![Uploading image.png…]()
![Uploading image.png…]()
- **Re-admissions by Department:** A bar chart showing that Ambulatory and Urgent Care have the highest re-admission counts.
- **Total Cost per Department:** A breakdown of revenue generated across different hospital wings.
- **Payer Distribution:** A pie chart showing the share of claims handled by Medicare, Medicaid, and private payers.

## 11. Key Insights
- **High Volume Departments:** Ambulatory services account for the largest portion of encounters (over 8,000 re-admissions).
- **Cost Drivers:** Inpatient and Urgent Care represent a significant portion of the total claim costs despite lower volumes compared to Ambulatory care.
- **Demographic Trends:** A significant portion of the patient base is concentrated in the Suffolk County/Boston area.

## 12. Recommendations
- **Resource Allocation:** Increase staffing in Ambulatory and Urgent Care during peak periods identified in the time-series analysis.
- **Re-admission Strategy:** Investigate the high re-admission rates in the Ambulatory department to determine if post-discharge care protocols need adjustment.
- **Financial Optimization:** Review the "Cost Post Payer Coverage" to identify if certain demographics are facing higher out-of-pocket burdens.

## 13. Conclusion
The insights derived from the Massachusetts General Hospital dataset provide a roadmap for optimizing department-specific resources and improving patient throughput. By addressing re-admission trends, the hospital can enhance both patient satisfaction and financial stability.

## 14. Contact Information
- **LinkedIn:** [Insert Your LinkedIn Link Here]
- **Email:** [Insert Your Email Here]
