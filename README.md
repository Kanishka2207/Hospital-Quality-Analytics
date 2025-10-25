# Hospital-Quality-Analytics
Hospital Quality &amp; Spending Analytics — CMS Open Data: A weekend project using public CMS datasets to explore the relationship between hospital quality ratings, mortality outcomes, and Medicare spending.

**Goal:** Evaluate how hospital quality ratings, mortality, and Medicare spending interact across 6,000+ U.S. hospitals using open CMS datasets.
Built entirely in **Python (Google Colab)** — fully reproducible, no local setup.

## Objectives
- Clean and merge CMS datasets: Hospital Info, Complications & Deaths, MSPB (Spending).
- Analyze whether higher spending improves hospital outcomes.
- Build predictive models for identifying high-performing (≥4-star) hospitals.
- Create a dashboard-ready dataset for **Tableau visualization**.
## Tools
| Category | Tools |
|-----------|--------|
| Data | CMS Open Data |
| Languages | Python 3 |
| Libraries | Pandas, NumPy, Plotly Express, Scikit-learn |
| Visualization | Tableau Desktop / Tableau Public |
| Environment | Google Colab |

## Workflow Overview
1. **Data Cleaning** — normalized 3 public CMS datasets, merged on hospital ID (CCN).  
2. **Exploratory Analysis** — star ratings, mortality, and spending distribution.  
3. **Predictive Model** — logistic regression with AUC ≈ 0.75 for 4+ star hospitals.  
4. **Dashboard Export** — generated `hospital_dash.csv` for Tableau visualization.

## Key Insights
- **Higher spend ≠ higher quality** — hospitals with lower MSPB often had better outcomes.  
- **Regional variation:** Midwest hospitals averaged 4.2 stars; Southern hospitals averaged 3.5.  
- **Efficiency gap:** top 25% hospitals spent 12% less per beneficiary while keeping mortality 15% lower.  
- Predictive model reached **AUC = 0.75**, identifying 3 of 4 high-performing hospitals.

##Dashboard Visuals

### Before (Prototype Design)
This initial prototype guided the final Tableau dashboard layout.  
[https://github.com/Kanishka2207/Hospital-Quality-Analytics/blob/c5487bf802a0da23f9d8d2e0bceffb9cd2399555/Prototype.png]

### After (Published Dashboard)
Final dashboard published on Tableau Public:  
[https://public.tableau.com/authoring/Hospital-Quality-Analytics/Dashboard1#1](https://public.tableau.com/authoring/Hospital-Quality-Analytics/Dashboard1#1)


## Tableau Sheets Overview

| Sheet | Description |
|-------|--------------|
| **KPI Summary** | Displays total hospitals, avg proxy stars, mortality, and MSPB. |
| **Map** | Filled map of states colored by average proxy stars. |
| **Scatter Plot** | Mortality vs Spending (colored by Proxy Stars). |
| **Bar Chart** | Top 10 states by average Proxy Stars. |
| **Detail Table** | Hospital-level breakdown with filters for State, Type, Ownership. |

---

## Author
**Kanishka Patel**  
Data & Analytics Professional  



