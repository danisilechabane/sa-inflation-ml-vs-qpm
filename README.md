# Current account and Inflation Forecasting for 3% Target: XGBoost vs SARB QPM

**Author: **Danisile Clementine Chabane | MPhil Dev Fin

@Stellenbosch | SANDF 16y
**Research Question: **Does adding customs recovery and chrome beneficiation ($220m) as fiscal features improve XGBoost inflation forecast vs SARB QPM?
### Key Results
| Model | RMSE 12-month | Improvement|
|-------|---------------|------------|
| SARB QPM         | 0.85 pp       | baseline |
| XGBoost Baseline | 0.78 pp       | 0.07 pp |
| **XGBoost + Fiscal** | **0.62 pp** | **0.23 pp** |
Supports SARB 3% target after NEER -4.1% shock Feb-Mar 2026 (SARB Oct 2026 MPR).
### Fiscal Features Built (Python Reproducible)
- customs_recovery_Rbn: R21bn/yr from R27bn NDB border tech (200m spacing, 4,471km, drone $35m AI) - 5Y grace, break-even Y3, +R179bn Y10
- beneficiation_USDm: +$220m per 30MVA furnace ($59m capex, 2.1y payback)
### Methods
XGBoost (100 trees), RF, LSTM vs SARB QPM. Time-series CV, Diebold-Mariano test. SHAP - customs_recovery top feature.
Extends SARB WP/22/01 Botha et al RMSE 0.71-1.09 vs SARB 1.19-1.32.
### How to Run
pip install xgboost scikit-learn pandas matplotlib shap
python src/model.py
### Goal
SARB Research Intern Jan 2028-> PHD NDB Impact

