# Green Valley Medical Center: Clinical Operations & Patient Outcomes Analysis

Author: Peret Brenda Dadah
Tool: Excel · Power Query · Power Pivot · DAX
Data source: Fictional healthcare dataset, built for educational and portfolio purposes
Scope: 400 admissions · 7 departments · 10 physicians

**Portfolio Disclaimer:** Green Valley Medical Center, all clinicians, patient records, and associated information are fictional and do not represent any real healthcare organisation or individual.

## Project Highlights

✔ Interactive Excel Dashboard ✔ Five KPI Tiles · Six Pivot Charts · Four Slicer Panels ✔ Cost-Efficiency Analysis by Treatment Pathway
✔ Power Query Data Preparation ✔ Case-Mix-Aware Reporting Caveats ✔ Six Targeted Executive Recommendations

## The Question

Which departments, treatments, and physicians are producing strong patient outcomes relative to cost, and where is spend rising without a matching improvement in recovery?

## Business Problem

Green Valley Medical Center collects patient data across seven departments but had no structured way to compare department performance, evaluate treatment effectiveness, or track whether rising costs were matched by better outcomes. Staffing, treatment, and budget decisions were being made without a shared evidence base. This project builds that evidence base using an Excel-based analytics workflow, while being explicit about where the data can and cannot support a firm conclusion.

## Key Findings

- **Cost-per-recovery-point is calculated at the group level** — a department or treatment's average cost divided by its average recovery score — not as a per-patient ratio averaged afterward. Conflating the two would understate genuine cost-efficiency differences between pathways.
- **Recovery scores are not adjusted for case mix.** Departments and physicians treat patients of differing severity, so a lower score may reflect a sicker patient population rather than weaker care. Every department- and physician-level finding is reported as a pattern flagged for review, not a proven performance gap.
- **Small cohorts are disclosed, not smoothed over.** Infant (n=2) and Other-gender (n=5) admissions appear in the underlying data for completeness but are excluded from headline findings too small a sample to support any conclusion.
- **Cost and outcome don't move together linearly.** High-cost admissions cost 10.6x more than low-cost admissions but the recovery gap between them is only 4.1 points a pattern that would be lost in a report that only tracked total spend rather than spend against outcome.

## Dashboard

The workbook contains one interactive executive dashboard with three panel groups:

**Departmental Performance** — recovery score vs. hospital stay by department, patient volume by gender

**Treatment & Physician Outcomes** — treatment pathway efficacy vs. facility baseline, recovery score by physician, recovery index by age group

**Financial Risk** — patient distribution by cost category, cost vs. recovery quadrant analysis

![Green Valley Medical Center dashboard](dashboard-screenshot.png)

## Technical Build

**Data model:** Single fact table (400 admissions) with two calculated dimension fields added — Age Group (seven life-stage cohorts) and Cost Category (Low / Medium / High) built and validated in Power Pivot

**Power Pivot / DAX Measures:** Average recovery score, average treatment cost, average stay, and cost-per-recovery-point, each sliceable by department, treatment type, physician, and age cohort

**Power Query:** Used for data cleaning and preparation — duplicate checks, categorical field standardisation, and calculated-field creation across all 400 records

## Skills Demonstrated

Excel · Power Pivot · DAX · Power Query · Data Modelling · Data Cleaning · Data Validation · Health Data Analytics · Executive Reporting · Data Storytelling

## Files in This Repository

| File | Description |
|---|---|
| [`green-valley-medical-center-performance-report.docx`](./green-valley-medical-center-performance-report.docx) | Full executive report: methodology, department/treatment/physician/demographic breakdowns, financial risk analysis, and six targeted recommendations |
| [`hospital_patient_dataset_400.xlsx`](./hospital_patient_dataset_400.xlsx) | Source dataset (400 admissions) and interactive Excel dashboard |
| [`dashboard-screenshot.png`](./dashboard-screenshot.png) | Dashboard export (PNG) |

## About Me

I'm a physician and public health specialist with over 14 years of experience strengthening health systems through programme management, monitoring & evaluation, and data-driven decision-making.

Today, I am building solutions at the intersection of Health Data, Digital Health, AI Governance, and Project Leadership.

This project reflects how I approach analytics: not just building dashboards, but being explicit about where the underlying data supports a firm conclusion and where it only supports a flag for further review.

## Let's Connect

LinkedIn: https://www.linkedin.com/in/pbdadah

Open to opportunities in:
Health Data Analytics
Digital Health
Business Intelligence
Health Informatics
AI-enabled Health Systems
