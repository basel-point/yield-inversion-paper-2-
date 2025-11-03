# Paper 2 — Logit: Recession Probability from the Yield Curve (12-Month Horizon)

**Purpose**  
This repository provides the technical materials and figures that accompany the Substack article, without exposing the full implementation details.

**Companion article:** “When the Curve Speaks: Estimating Recession Risk with a Logistic Classification Model”  
https://thebaselpoint.substack.com/p/when-the-curve-speaks

## Summary
We estimate a 12-month-ahead U.S. recession probability using a logistic classification model with yield-curve spreads. The preview here presents results, method notes, and selected figures. Full implementation is withheld.

**Method (brief):**
- Predictors: 10Y–3M and 10Y–2Y spreads
- Lags: 1-month and 6-month
- Evaluation: expanding-window (walk-forward)
- Outputs: ROC/AUC, precision/recall snapshot, full-history probability with NBER shading, and a recent-window view

## Figures
- `figures/recession_prob_12m_full.png`
- `figures/recession_prob_12m_last_8y.png`
- `figures/roc_walk_forward.png`
- `figures/confusion_matrix_fed_style.png` 

## Data Sources
- Federal Reserve Economic Data (FRED) for Treasury yields and the NBER recession indicator.
- Additional macro sources as referenced in the article.
  
No raw data files are included in this repository.

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


