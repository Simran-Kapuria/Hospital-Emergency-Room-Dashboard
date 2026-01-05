# Hospital Emergency Room Dashboard | Excel, Power Pivot, Power Query & Power BI Concepts

## Project Overview
This project focuses on building an end-to-end Hospital Emergency Room Analysis Dashboard to monitor patient flow, waiting time, admission status, and department referrals.  
The dashboard helps hospital stakeholders improve operational efficiency, reduce patient wait time, and enhance overall service quality.

The complete solution was developed using advanced Excel features along with Power Pivot, Power Query, and Power BI-style data modeling concepts.

---

## Tools & Technologies Used
- Microsoft Excel
- Power Query (Data Cleaning & Transformation)
- Power Pivot (Data Modeling)
- DAX Measures & Calculated Columns
- Pivot Tables & Pivot Charts
- Slicers & Timeline Filters
- Dashboard Design & Data Visualization

---

## Project Objectives
- Analyze emergency room patient inflow
- Track patient waiting time and service delays
- Understand admission vs non-admission trends
- Identify high workload departments
- Analyze patients by age group and gender
- Support data-driven decision-making in healthcare operations

---

## Key KPIs
- Total Number of Patients
- Average Waiting Time
- Patient Satisfaction Score
- Percentage of Patients Attended Within 30 Minutes
- Admission vs Not Admitted Status
- Gender-wise Patient Distribution
- Age Group Analysis
- Department Referral Analysis

---

## Data Modeling & Transformation
- Cleaned and transformed raw hospital data using **Power Query**
- Created a **Calendar Table** for time-based analysis
- Built relationships using **Power Pivot**
- Optimized data model for accurate reporting

### Calendar Table (Power Query)

List.Dates(#date(2023,01,01), 731, #duration(1,0,0,0))

---

## DAX Calculations
### Age Group Classification
IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))


### Patient Attend Status
IF([Patient Waittime] < 30, "Within Time", "Delay")

---

## Dashboard Insights
- Majority of patients were attended within the target time
- Age group 30–49 shows the highest emergency visits
- General Practice department receives maximum referrals
- Slight dominance of male patients observed
- Admission rate is almost evenly split, indicating balanced ER utilization

---

## Dashboard Preview
The complete dashboard screenshot is included in this repository for reference.

---

## Conclusion
This project demonstrates my ability to build an end-to-end analytical dashboard using Excel, Power Query, Power Pivot, and DAX.  
It highlights my skills in data cleaning, modeling, analysis, and visualization with real-world healthcare data.

---

## Author
**Simran Kapuria**  
Aspiring Data Analyst | Excel | Power BI | SQL | Python
