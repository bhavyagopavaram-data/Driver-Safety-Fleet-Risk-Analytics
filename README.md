# Driver Safety & Fleet Risk Analytics

**Author:** Bhavya Sri Gopavaram  
**University:** DePaul University- MS in Business Analytics  
**Tools:** Python | Pandas | SQL | Scikit-learn | Matplotlib | Seaborn | Jupyter  
**Dataset:** 321,439 real fleet telematics events | 176 features | 2 companies  

---

## Project Overview

An end-to-end fleet risk analytics pipeline built on real telematics data from a Master's capstone project. This project covers the full data analyst workflow from raw data ingestion and cleaning, through exploratory analysis, KPI development, statistical modeling, SQL querying, and executive-level business recommendations.

---

## Business Problem

Fleet operators face significant financial and safety risk from unsafe driver behavior. This project was designed to answer five core business questions:

- Which drivers pose the highest operational risk?
- Which behaviors most strongly predict high-risk events?
- Does structured coaching actually reduce violations- and by how much?
- Which states and vehicle types carry the most exposure?
- Can we proactively identify drivers who will need coaching before incidents occur?

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Pandas | Data cleaning, transformation, aggregation |
| Matplotlib / Seaborn | Charts, visualizations, dashboards |
| Scikit-learn | Linear regression, logistic regression, model evaluation |
| pandasql | SQL queries on DataFrames (standard SQL syntax) |
| Jupyter Notebook | Interactive end-to-end analysis environment |

---

## Analysis Pipeline — 16 Sections

| Section | Description |
|---|---|
| 1. Data Cleaning | Removed nulls, zero columns, standardised 176 features |
| 2. Data Loading | Loaded and validated 321,439 rows of telematics data |
| 3. KPI Framework | Total events, coachable rate, average event score by company |
| 4. State Analysis | Top 10 high-risk states overall and by company |
| 5. Vehicle Analysis | Events and coachable rate by vehicle type |
| 6. Safety Categories | 11 violation categories with severity scoring |
| 7. Driver Risk | High / Medium / Low risk driver classification |
| 8. Time Patterns | Violations by hour, day of week, and season |
| 9. Correlation Analysis | Pearson correlation of behaviors vs event scores |
| 10. Linear Regression | Event score prediction model |
| 11. Logistic Regression | Coachable event prediction model |
| 12. Company Comparison | Side-by-side Company 1 vs Company 2 analysis |
| 13. Coaching Effectiveness | Pre vs post coaching violation reduction |
| 14. Future Prediction | Top 20 drivers predicted to need coaching |
| 15. Recommendations | 5 data-driven business actions |
| 16. SQL Analysis | 8 business questions answered using SQL |

---

## Machine Learning Results

| Model | Target Variable | R2 | Accuracy | Correlation |
|---|---|---|---|---|
| Linear Regression | Event Score | 91.5% | - | 0.955 |
| Logistic Regression | Coachable Event | - | 97.35% | AUC 0.98 |

**Top predictors of risk:** Overall behaviors, fundamental violations, driver awareness, driver condition, traffic violations

---

## Key Findings

- Overall unsafe driving behaviors show the strongest correlation (0.636) with high event scores
- Structured coaching reduces risky behaviors by 90-100% in both companies
- Company 2 shows stronger model fit (R2 = 92.1%) and stricter coaching enforcement
- Following distance violations are the single most common trigger for coaching sessions
- Repeat offenders can be proactively identified with 97%+ predictive accuracy

---

## SQL Queries — Business Questions Answered

| Query | Business Question |
|---|---|
| Query 1 | What are the KPIs per company? |
| Query 2 | Which states are highest risk? |
| Query 3 | Who are the top 20 most dangerous drivers? |
| Query 4 | What hours of the day have the most violations? |
| Query 5 | Does coaching actually reduce violations? |
| Query 6 | Which vehicle types are highest risk? |
| Query 7 | Are violations increasing or decreasing over time? |
| Query 8 | Which drivers re-offended after coaching? |

All queries written in standard SQL compatible with PostgreSQL, Snowflake, MySQL, and BigQuery.

---

## Business Recommendations

1. **Focused Coaching Modules** - Build trigger-specific training for the top 10 high-risk behaviors identified in the data
2. **Mandatory Simulation Training** - Require repeat offenders to complete AI-driven driving simulation before returning to live routes
3. **State-Level Coaching Strategy** - Deploy intensive coaching programs in highest-violation states (TX, CA, IL)
4. **Performance Incentive Program** - Introduce bonuses and recognition for drivers with clean safety records
5. **Real-Time Ride-Along Coaching** - Implement live coaching interventions for drivers with recurring high-risk patterns

---

## Repository Structure

```
Driver-Safety-Fleet-Risk-Analytics/
├── Driver_Safety_Fleet_Risk_Analytics.ipynb    # Full analysis notebook
└── README.md                                   # Project documentation
```

**Note:** The dataset is proprietary fleet telematics data from a DePaul University Master's capstone project and is not included in this repository.

---

## About

This project was completed as the capstone for a Master of Science in Business Analytics at DePaul University. It demonstrates end-to-end data analyst capabilities including data engineering, exploratory analysis, KPI development, statistical modeling, SQL querying, and executive communication of insights.
