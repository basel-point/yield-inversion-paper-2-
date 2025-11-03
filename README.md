# Paper 2 — Logit: Recession Probability from the Yield Curve (12-Month Horizon)

This repository provides the technical companion materials for the article published on *The Basel Point* Substack:

📘 **Companion Article:**  
[*When the Curve Speaks: Estimating Recession Risk with a Logistic Classification Model*](https://thebaselpoint.substack.com/p/when-the-curve-speaks)

---

## Repository Contents

- `notebooks/Paper2_Logit_Recession_12m_preview.ipynb` — *Redacted preview notebook.*  
  Demonstrates methodology and outputs for the logistic regression model used to estimate recession probabilities from the yield curve.  
  Full implementation details and certain code sections have been intentionally withheld.

- `/figures/` — contains static output charts referenced in the notebook, including the ROC/AUC curve, probability series with NBER shading, and precision/recall plot.

---

## Method Overview

Logistic regression model with an expanding-window (walk-forward) backtest to predict the NBER recession indicator (`USREC`) 12 months ahead.  
Predictors include the 10Y–3M and 10Y–2Y Treasury spreads, along with 1- and 6-month lags.

---

## Expected Data Files

- `yields_monthly.csv` (or `treasury_yield.csv`) with columns:  
  `Date`, `3m (DGS3MO)`, `2y (DGS2)`, `10y (DGS10)` — monthly averages or end-of-month; `Date` in `YYYY-MM-DD`.  
- `usrec_monthly.csv` with columns:  
  `Date`, `USREC` (NBER recession indicator; 1 = recession, 0 = expansion).

---

## Environment

- Jupyter Notebook
- pandas
- numpy
- matplotlib
- scikit-learn
- statsmodels


---

## Access

Full notebooks and datasets are available upon request for professional review.  
Please contact **thebaselpoint@gmail.com**.

---

© 2025 *The Basel Point Research.*  
Prepared by **S.Y. Kim**.  
All rights reserved.


