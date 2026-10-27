# ML vs Traditional Models Nowcasting SA Inflation: ERPT & Oil Shocks
**Status: **APPLICATION for MCom Economics 2027 @Stellenbosh University - Not yet admitted
**Author: **Danisile Clementine Chabane | SU Alumnus BHons ORM NQF 8 Econ Major | BAdmin Econ UNISA | 16y SANDF
**Alignment: BER @ Stellenbosch (Exchange Rate Research) 2027
**Disclaimer: **Independent preparatory research for MCom 2027 application. Not affiliated with SU MCom program yet.
**Research Question: **Do ML models (XGBoost, RF LSTM) outperform traditional models (ARIMA, VAR, SARB QPM) in nowcasting SA CPI when incorporating Exchange Rate Pass-Through and Oil Shocks under SARB 3% target?
### Key Results
| Model | RMSE 12-month | Improvement|
|-------|---------------|------------|
| SARB QPM | 0.85 pp       | baseline |
| XGBoost Baseline | 0.78 pp       | 0.07 pp |
| **XGBoost + BER + ERTP + Oil** | **0.62 pp** | **0.23 pp (27%)** |
Supports SARB 3% target. Uses BER Inflation Expectations Survey housed at SU Dept of Economics.
### Data Built (Python Reproducible) 
- CPI (StatsSA), USD/ZAR (SARB), Brent (FRED), Repo (SARB), BER Inflation Expactations, DMRE Fuel, Output Gap 2010 - 2026
- No customs/beneficiation - pure ERTP & Oil focus for BER mandate
### Methods
XGBoost (100 trees), RF, LSTM vs SARB QPM. Time-series CV, Diebold-Mariano test. SHAP - ERTP top feature.
Extends SARB WP/22/01 Botha et al RMSE 0.71-1.09 vs SARB 1.19-1.32.
### Alignment with SU MCom 2027
- Compulsory: Macroeconomics (20cr), Microeconomics (20cr), Econometrics (20cr) - Intensive Stats 60% required
- Electives: Data Science for Economics & Finance (Sem1) - Coursera Python Certificate supports, advance Time-Series Econometrics
- Research Assignment (60cr)
### Technical upskilling
Coursera Python for Data Science Certificate (In Progress)
Stack: Python, Pandas, Scikit-Learn, XGBoost, SHAP
### How to run
pip install xgboost scikit-learn pandas matplotlib shap
Python src/model.py
### Career Goals & Contribution to South Africa
**Long-Term Goal (2027-2032):**To work with Bureau for Economic Research (BER) @ Stellenbosch University and SARB Research Department on policy-relevant research based on this topic
**How this research helps South Africa:**
1. **Inflation Targeting: ** Improve SARB QPM nowcasting accuracy from RMSE 0.85 TO 0.62 using BER Expectations + ERPT + Oil Shocks = Better support for SARB 3% inflation target and price stability.
2. **Rand Appreciation Pathway: **By quantifying Exchange Rate Pass-Through (ERTP) accurately, this model identifies conditions where ZAR appreciation is sustainable (via lower import costs, anchored BER expectations, reduced oil pass-through) - supporting stronger Rand and lower inflation.
3. **BER Mandate: ** Directly extends BER's core work on Inflation Expectations Survey (housed at SU Department of Economics) into Machine Learning nowcasting for monetary policy.
4. **Policy Pipeline: This MCom Research Assignment (60cr) is intended to evolve into a BER Working Paper and SARB collaborative research during MCom 2027 - 2028 and beyond.
**Intended Role: **Research Economists | Data Scientists @BER/SARB/National Treasury - Bridging Academic Research (SU MCom 2027) + Python (Coursera ) + Policy.
> As SU Alumnus BHons ORM Econ Major NQF 8 and 16y SANDF service, my commitment is to use this research to contribute to South Africa macro stability - low inflation, stable Rand, and BER/SARB research excellence.
