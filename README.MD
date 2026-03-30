# HR Analytics in Power BI — Case Study

A 6-page Power BI report built around Atlas Labs, a fictitious software company. The brief: import and analyze HR data, identify what's driving a 16.1% attrition rate, and deliver a set of concrete recommendations for retaining employees.

Built as part of the [HR Analytics in Power BI](https://www.datacamp.com/courses/case-study-hr-analytics-in-power-bi) case study on DataCamp.

---

## The Problem

Atlas Labs has **1,470 employees**, of which **237 have left** — a 16.1% attrition rate. The report doesn't stop at that number. It works through the workforce by department, age, demographics, travel habits, overtime, tenure, and individual performance to figure out where the problem is concentrated and what's causing it.

---

## Dashboard Pages

### Page 1 — Overview
- Total employees: **1,470** | Active: **1,233** | Inactive: **237**
- Overall attrition rate: **16.1%**
- Active employees by department:
  - Technology: **828**
  - Sales: **354**
  - Human Resources: **51**
- Treemap of active employees by department and job role — Software Engineers, Data Scientists, and Machine Learning Engineers make up the bulk of Technology headcount
- Dual-axis chart: total employees and attrition rate by age band
  - Attrition peaks in the **20–29** age group
  - Drops steadily through 30–39 and 40–49
  - Near-zero for employees under 20 and over 50

### Page 2 — Demographics
- Age range: youngest employee **18**, oldest **51**
- Employee count by age band:
  - 20–29: **874** (largest group)
  - 30–39: **289**
  - 40–49: **219**
  - Under 20: **81**
  - 50+: **7**
- Gender breakdown per age band (Female, Male, Non-Binary, Prefer Not To Say)
- Marital status: Married **624** | Single **549** | Divorced **297**
- Ethnicity and average salary — White is the largest group; salary variance across ethnicities is visible but relatively narrow (range ~$100K–$120K average)

### Page 3 — Demographics 2 (Attrition Cuts)
- Attrition by marital status:
  - Single: **23.3%** — significantly higher than others
  - Married: **12.7%**
  - Divorced: **10.1%**
- Attrition by gender:
  - Male: **17.5%**
  - Female: **15.4%**
  - Non-Binary: **15.3%**
- Attrition by education field:
  - Technical Degree: **31.6%** — highest by a wide margin
  - Human Resources: **25.9%**
  - Business Studies: **21.3%**
  - Marketing: **20.0%**
  - Computer Science / Information Systems: **13.4% / 12.9%**
- Attrition by education level:
  - No Formal Qualifications: **18.2%**
  - Bachelor's: **17.3%**
  - High School: **15.6%**
  - Master's: **14.6%**
  - Doctorate: **10.4%** — lowest attrition

### Page 4 — Attrition Deep Dive
- **16.1%** overall rate displayed as anchor KPI
- Attrition by department (dual-axis — rate and headcount):
  - Sales: highest rate
  - Human Resources: mid
  - Technology: **13.8%** — lowest of the three
- Attrition by hire date (2012–2022): rate fluctuates between ~10–20%, with visible spikes around 2016 and 2020
- Attrition by travel frequency:
  - Frequent Travellers: highest churn — above 20%
  - Some Travel: moderate
  - No Travel: lowest — under 10%
- Attrition by overtime:
  - Employees required to do overtime churn at roughly **double** the rate of those who aren't
- Attrition by tenure:
  - Peaks sharply in the first 0–2 years at the company
  - Drops significantly after year 5 and stabilizes

### Page 5 — Performance Tracker (Individual View)
- Employee selector dropdown — example shown: **Celestine Kyngdon**
  - Start Date: 04/23/2017
  - Last Review: 02/09/2022
  - Next Review: 02/09/2023
- Six tracked metrics over time (line charts, 2010–2022):
  - Job Satisfaction
  - Relationship Satisfaction
  - Self Rating
  - Work Life Balance
  - Manager Rating
  - Environment Satisfaction
- Rating scales (for reference):
  - Satisfaction: Dissatisfied (2) → Neutral (3) → Satisfied (4) → Very Satisfied (5)
  - Performance: Needs Improvement (2) → Meets Expectation (3) → Exceeds Expectation (4) → Above and Beyond (5)
- This page makes it possible to track whether an individual employee's engagement is trending up or down over time — useful for flagging flight risks before they leave

### Page 6 — Attrition Explainer & Action Plan
- Drillable view by department, job role, and age band
- Sales highlighted:
  - Overall Sales attrition: **20.6%**
  - Sales Representatives: **39.8%** — the single highest job role attrition in the company
  - Sales Executives: **17.5%**
  - Managers: **5.4%**
  - Highest risk age band in Sales: **20–29 at 21.5%**

Employee Retention Action Plan (built into the report):
- Cap and redistribute excessive overtime hours across teams
- Introduce meaningful recognition and flexibility initiatives
- Target financial wellness benefits for lower-wage bands
- Offer commute relief: remote days, transit subsidies, relocation support
- Strengthen onboarding and the first-90-day experience
- Expand mental health resources and career development pathways
- Implement living-wage adjustments or bonus structures for entry-level roles
- Hybrid/WFH options for employees with commutes over 1 hour
- Dedicated mentorship programs and "quick wins" tracks for new hires

---

## Key Findings

- **Sales Representatives churn at 39.8%** — the most urgent retention problem in the company
- **Overtime is a major driver** — employees required to work overtime churn at roughly twice the rate of those who don't
- **The first two years are critical** — attrition spikes sharply at low tenure and drops off significantly after year 5
- **Technical Degree holders** have the highest attrition by education field (31.6%) — likely a competitive external market for that skill set
- **Single employees churn more** (23.3%) than married (12.7%) or divorced (10.1%)
- **Frequent travel correlates with higher attrition** — above 20% vs. under 10% for non-travelers
- **Doctorate holders are the most stable** employee segment at 10.4% attrition

---

## Files

```
├── HR_Analytics_Atlas_Labs.pbix
├── HR_Analytics_Atlas_Labs.PDF
├── README.md
├── certificate/
│   └── hr_analytics_powerbi_certificate.pdf
├── datasets/
│   ├── employees.csv
│   ├── performance_ratings.csv
│   └── education_levels.csv
└── screenshots/
    ├── 01_overview.png
    ├── 02_demographics.png
    ├── 03_demographics2_attrition.png
    ├── 04_attrition_deepdive.png
    ├── 05_performance_tracker.png
    └── 06_explainer_action_plan.png
```

---

## How to Open

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) — free
2. Clone the repo
3. Place datasets in `/datasets/` and update data source paths in Power BI if prompted
4. Open `HR_Analytics_Atlas_Labs.pbix`

---

## Course

[Case Study: HR Analytics in Power BI](https://www.datacamp.com/courses/case-study-hr-analytics-in-power-bi) — DataCamp
