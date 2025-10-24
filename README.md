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

