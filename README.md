# workforce-demand-headcount-capacity-analytics
End-to-end workforce analytics project analyzing demand, headcount, staffing capacity, coverage, overtime, absenteeism, operational performance, and staffing scenarios using Excel, Power Query, SQL, Power BI, and DAX.
# Workforce Demand, Headcount & Capacity Analytics

## Overview

I built this project to explore a practical workforce planning question:

> **Do we have enough people, at the right time, to meet operational demand?**

In high-volume operations, staffing is not simply about how many employees are available. Demand changes throughout the day, employees may be absent, overtime can increase, and performance can be affected when capacity falls below operational requirements.

This project brings those factors together into one analytical model.

Using a simulated 12-month workforce dataset with 4,200+ records, I analyzed demand, required headcount, available capacity, staffing gaps, coverage, overtime, absenteeism, and operational performance.

The analysis was developed using **Excel, Power Query, Power BI, DAX, and SQL**.

---

## The Business Question

The main question behind the project was:

**How can workforce data be used to identify capacity constraints before they become an operational problem?**

To investigate this, I looked at several connected questions:

* Is available headcount keeping up with operational demand?
* When do staffing shortages occur?
* Which shifts or operational areas experience the greatest pressure?
* Is overtime being used when workforce capacity is insufficient?
* What happens if demand increases?
* What happens if absenteeism increases?
* Would adding one FTE materially improve coverage?

Rather than looking at each metric separately, I wanted to understand the relationship between **demand, workforce capacity, and operational performance**.

---

## What I Analyzed

The dataset contains operational and workforce information including:

* Date
* Location
* Operational Area
* Shift
* Hour
* Demand Volume
* Required HC
* Scheduled HC
* Available HC
* FTE Capacity
* Absences
* Overtime Hours
* Staffing Gap
* Coverage %
* Operational Posture
* Performance Target
* Actual Performance

I also created scenario fields to test how the workforce responds when operating conditions change.

---

## Analytical Approach

The analysis follows a simple business logic:

**Demand**


**Required Workforce**


**Available Workforce**


**Staffing Gap & Coverage**


**Operational Performance**

This helped me move beyond simply reporting headcount and instead look at whether workforce capacity was actually aligned with operational requirements.

### Staffing Gap

I used:

**Available HC − Required HC**

A negative value indicates that available workforce capacity is below the estimated requirement.

### Coverage

I used:

**Available HC ÷ Required HC**

This provides a simple view of how much of the required workforce capacity is currently available.

---

## Scenario Analysis

One of the main parts of the project is testing what happens when the operating environment changes.

### 1. Demand +10%

I increased demand by 10% and evaluated the resulting:

* Required HC
* Staffing Gap
* Coverage %

This helps illustrate the workforce impact of a potential increase in operational volume.

### 2. Absences +20%

I increased absences by 20% to understand how sensitive available capacity is to absenteeism.

The analysis evaluates:

* Available HC
* Staffing Gap
* Coverage %

### 3. Add +1 FTE

I also tested a simple staffing intervention:

**What happens if one additional FTE is added?**

This allows the potential coverage improvement to be compared against the baseline situation.

---

## Dashboard Results


The current analysis provides an overall view of workforce and operational performance.

| KPI                        | Current Result |
| -------------------------- | -------------: |
| Average Actual Performance |         91.70% |
| Performance Target         |         92.40% |
| Average Coverage           |         92.40% |
| Average Staffing Gap       |       -0.57 HC |
| Average FTE Capacity       |           7.78 |
| Average Overtime           |     1.44 hours |

One of the observations from the current model is that **actual performance is below the stated performance target**, while the average staffing gap is also negative.

That creates an important analytical question:

> **Are periods of insufficient workforce coverage contributing to weaker operational performance?**

The dashboard allows this relationship to be investigated across time, shifts, locations, and operational areas rather than assuming that staffing is the only cause.

---

## Excel Analysis

I used **Excel and Power Query** to prepare and analyze the workforce dataset.

The Excel component includes:

* Data preparation
* Workforce calculations
* KPI analysis
* Scenario calculations
* Operational dashboard

Excel provides the detailed analytical workbook behind the project.

---

## Power BI Analysis
<img width="1830" height="985" alt="image" src="https://github.com/user-attachments/assets/d7ec5506-6617-450e-bf38-f6b606ebfbca" />
<img width="1266" height="593" alt="image" src="https://github.com/user-attachments/assets/ed28838f-c92f-4195-864c-0e5d875fdc78" />
<img width="930" height="741" alt="image" src="https://github.com/user-attachments/assets/c7034885-454b-4fd4-a3d7-8473b107609b" />




I used **Power BI and DAX** to create an interactive view of the same workforce problem.

The Power BI analysis focuses on:

* Demand and capacity
* Required vs. available headcount
* Staffing gaps
* Coverage
* Overtime
* Absenteeism
* Operational performance
* Workforce scenarios

The purpose of the dashboard is not just to display numbers, but to allow the user to explore **where capacity pressure occurs and how different workforce conditions affect operations**.

---

## What This Project Demonstrates

This project demonstrates my approach to solving a business problem with data:

**1. Start with the operational question**

What workforce capacity is actually required?

**2. Structure the data**

Bring demand, staffing, availability, and performance information together.

**3. Build measurable KPIs**

Translate the operational problem into staffing gap, coverage, overtime, absenteeism, and performance metrics.

**4. Test different conditions**

Use scenarios to understand workforce sensitivity.

**5. Visualize the results**

Use Excel and Power BI to make the analysis easier to explore.

**6. Translate analysis into decisions**

Use the results to identify where staffing, capacity, or operational planning may need attention.

---

## Tools

**Excel**
Detailed analysis, calculations, KPI development and dashboarding.

**Power Query**
Data cleaning, transformation and preparation.

**Power BI**
Interactive reporting and visualization.

**DAX**
Measures and analytical calculations within Power BI.

**SQL**
Data analysis and validation.

---

## Dataset

The dataset is **simulated** and was created specifically for this portfolio project.

It represents a 12-month operational workforce environment with 4,200+ records.

No confidential employer, employee, customer, or proprietary operational data is included.

---

## Repository

```text
Workforce-Demand-Headcount-Capacity-Analytics/
│
├── README.md
│
├── Excel/
│   └── Workforce_Analytics.xlsx
│
├── PowerBI/
│   └── Workforce_Analytics.pbix
│
├── Data/
│   └── Workforce_Dataset.csv
│
├── SQL/
│   └── Workforce_Analysis.sql
│
└── Screenshots/
    ├── Excel_Dashboard.png
    └── PowerBI_Dashboard.png
```

---

## Skills Demonstrated

### Workforce & Operations Analytics

* Workforce planning
* Headcount analysis
* Capacity analysis
* Staffing gap analysis
* Coverage analysis
* Overtime analysis
* Absenteeism analysis
* Scenario planning
* Operational performance analysis

### Data & Business Intelligence

* Excel
* Power Query
* Power BI
* DAX
* SQL
* Data preparation
* KPI development
* Data visualization
* Dashboard development
* Analytical storytelling

---

## Final Takeaway

The main idea behind this project is simple:

> **Workforce planning is not just about headcount. It is about matching capacity to demand while understanding the operational consequences of being over- or under-capacity.**

By combining workforce, demand, and performance data, the model provides a way to identify staffing pressure, test potential scenarios, and support more informed workforce decisions.

---

## Author

**Jaspreet Dhatt**

Workforce Planning | Operations Analytics | Business & Data Analytics

This project reflects my interest in using data to understand operational problems, identify patterns, and turn analysis into practical business decisions.
