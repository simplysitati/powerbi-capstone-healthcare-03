# Power BI Capstone: Patient Flow Intelligence (Scenario 2)

Course: DSA3050 – Big Data & Data Visualization  
Semester: Summer 2025  
Group 03

## Team Members
- Wesley – Business Analyst & Repo Manager  
- Kemo – Data Model & DAX Architect  
- Abdirisak – Data Wrangler / ETL Lead

## Project Summary

This project focuses on optimizing emergency room (ER) operations across a regional hospital network using Power BI and DAX. We built an interactive dashboard that analyzes ER patient wait times, triage bottlenecks, staffing levels, and readmission risks.

Using a dataset of 5,000 simulated ER visits, we engineered a star schema model and developed metrics that enable ER administrators and hospital directors to visualize bottlenecks, predict operational pressure, and reduce avoidable readmissions.

## Objectives
- Visualize patient flow by time, urgency, and outcome
- Simulate staffing impact on ER efficiency
- Flag high-risk readmission patterns
- Enable real-time triage and shift decision-making

## Data Model

Fact Table: ER Visits  
Dimensions:
- Date  
- Triage Level  
- Patient  
- Hospital  
- Shift (simulated)  
- Region

## Key Metrics
- Average Time to Triage  
- Average Time to Doctor  
- Nurse-to-Patient Ratio  
- Patient Volume per Hour  
- Readmission Rate within 72 hours  
- Satisfaction Score by Shift  
- Outcome Breakdown (Discharged, Admitted, Referred)

## Dashboard Pages

### 1. Triage Flow & Bottlenecks
Purpose: Identify when and for whom the ER experiences the most pressure.
- Heatmap of visits by hour & day
- Avg wait time by urgency level
- KPI cards: Avg Wait Time, Time to Triage, Time to Doctor
- Volume trends across time of day and day of week

### 2. Staffing & Resource Utilization
Purpose: Evaluate staff sufficiency against patient volume and outcomes.
- Line chart: Patient volume vs nurse ratio
- Avg Specialist Availability and Satisfaction
- Outcome comparison by hospital
- Weekly specialist distribution trends


## Tools Used
- Power BI (Data Model + Visuals)  
- Power Query (ETL)  
- DAX (Custom Measures)  
- GitHub (Collaboration)

## View Dashboard
[[Click here to view published dashboard](link.txt)](https://app.powerbi.com/view?r=eyJrIjoiZGI2NzBlYzktN2FhYS00NjExLWFhNTctMWUzOTMxNDAyZGYwIiwidCI6IjE2ZDgzZWU2LTI1NGEtNDY5ZC1hNmNjLTU0ZTJjYTIzMTNlNyIsImMiOjh9)

## Dashboard Previews

### Triage Flow & Bottlenecks
![Dashboard 1](screenshots/triage_bottleneck_view.png)

Insights:  
- Peak patient load occurs late mornings (10 AM – 1 PM)  
- Low-urgency patients wait >170 mins on average  
- Monday & Tuesday are the busiest days  
- Overall ER wait time averages 81.92 mins

### Staffing & Outcome Intelligence
![Dashboard 2](screenshots/staffing_outcome_view.png)

Insights:  
- Specialist availability drops on weekends  
- Nurse-to-patient ratio averages 3.24  
- Satisfaction remains low despite consistent discharge rates  
- Uniform outcomes suggest systemic inefficiency across hospitals

## Project Structure

powerbi-capstone-healthcare-03/
├── data/
│   ├── raw/
│   └── cleaned/
├── pbix/
│   └── final_dashboard.pbix
├── screenshots/
│   ├── triage_bottleneck_view.png
│   └── staffing_outcome_view.png
├── documentation/
│   ├── business_case.md
│   ├── data_model_diagram.png
│   ├── ROI_calculations.xlsx
│   └── performance_tuning.md
├── README.md
├── link.txt

---

For submission or reference, contact Wesley Sitati (juswes).
