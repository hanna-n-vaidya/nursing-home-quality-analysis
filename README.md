# Nursing Home Analysis: What Drives Star Ratings Across U.S. States?

## Project Motivation

Families choosing nursing home care as well as nursing homes looking to improve their ratings need to understand what factors are contributing to these scores. This project uses Shapley values to determine relevant features for predicting a state's average nursing home star rating and fits a linear regression model with those features. 

---

## Business Questions

1. How are nursing home star ratings distributed across U.S. states?
2. What factors most contribute to overall ratings?
3. Which states have the best and worst overall ratings?

---

## Repository Contents

| File | Description |
|------|-------------|
| `nursing_home_analysis.ipynb` | Main Jupyter notebook with full CRISP-DM analysis |
| `NH_StateUSAverages_Jul2026.csv` | Source dataset from CMS |
| `README.md` | This file |

---

## Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, aggregation |
| `numpy` | Numerical operations, permutation sampling |
| `scikit-learn` | Imputation, RandomForestRegressor, cross-validation, metrics |
| `matplotlib` | Base plotting |
| `seaborn` | Statistical visualizations |

---


## Summary of Results

- Average state nursing home star ratings center around 3 stars.
- Hawaii has the highest average nursing home star ratings, while Guam has the lowest.
- Quality Measure rating, nurse aide staffing hours per resident, and percent of residents on antipsychotic medication contribute the most to average overall rating. QM rating and nurse aide staffing hours contribute positively to the score, while percent of residents on antipsychotic medication contribute negatively to the score.

---

## How to Run

```bash
git clone https://github.com/<your-username>/nursing-home-quality-analysis
cd nursing-home-quality-analysis
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook nursing_home_analysis.ipynb
```

---

## Acknowledgments

- **Dataset:** State US Averages, CMS (https://data.cms.gov/provider-data/dataset/xcdc-v8bm#data-table)
- **Project framework:** Udacity Data Scientist Nanodegree
