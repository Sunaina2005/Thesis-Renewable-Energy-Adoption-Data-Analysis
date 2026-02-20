# Modelling and Forecasting Global Renewable Energy Adoption

**Master's Thesis - IU International University of Applied Sciences**  
**Author:** Sunaina Manjunath  
**Program:** M.Sc. Computer Science  
**Year:** 2025

---

## Overview

This thesis analyzes renewable energy adoption patterns across 211 countries from 2000-2023, combining econometric analysis with machine learning to both explain drivers and predict future trends.

**Key Question:** Why do some countries adopt solar and wind energy rapidly while others lag behind, despite similar climate commitments?

---

## Research Objectives

1. Identify economic and demographic drivers of renewable energy capacity growth
2. Compare forecasting models (ARIMA, Prophet, XGBoost) for prediction accuracy
3. Apply explainable AI (SHAP) to interpret machine learning predictions
4. Cluster countries into adoption typologies based on structural characteristics

---

## Methodology

**Data Sources:**
- IRENA: Renewable capacity statistics (solar PV, onshore/offshore wind)
- World Bank WDI: GDP, population, electricity access, energy use
- REN21: Policy indicators
- Energy Institute: Cross-validation data

**Analytical Pipeline:**
1. Data cleaning and panel construction (211 countries × 24 years = 5,064 observations)
2. Fixed Effects panel regression for causal inference
3. Time-series forecasting (ARIMA, Prophet, XGBoost)
4. K-Means clustering with PCA
5. SHAP analysis for model explainability

**Tools:** Python 3.10 (pandas, statsmodels, linearmodels, scikit-learn, xgboost, shap, prophet)

---

## Key Findings

**Drivers of Adoption:**
- GDP per capita: +10% GDP → +7.5% renewable capacity
- Population size: Positive scale effect
- Electricity access: Infrastructure readiness matters
- Energy intensity: High fossil fuel use slows transition

**Forecasting Performance:**
- ARIMA: Most consistent (MAPE 0.2-2%)
- Prophet: Best for non-linear growth patterns
- XGBoost: Powerful but prone to overfitting on short series

**Country Typologies:**
- Developed Leaders (high-income, high-adoption countries)
- Emerging Giants (rapid growth)
- Resource-Rich Laggards (moderate income, slow adoption)
- Developing Strivers (low income, financing constraints)

---

## Repository Contents

- `Sunaina_Thesis_Data_Analysis.ipynb` - Complete analytical pipeline
- `Master Thesis github.pdf` - Full thesis document
- `requirements.txt` - Python dependencies

---

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/renewable-energy-adoption-thesis.git
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Download data:
   - [IRENA Capacity Statistics](https://pxweb.irena.org/pxweb/en/IRENASTAT)
   - [World Bank WDI](https://databank.worldbank.org/source/world-development-indicators)
   - [REN21 Data Pack](https://www.ren21.net/reports/)
   - [Energy Institute Review](https://www.energyinst.org/statistical-review)

4. Open and run `Sunaina_Thesis_Data_Analysis.ipynb`

---

## Citation

If you use this work, please cite:
```
Manjunath, S. (2025). Modelling and Forecasting Global Renewable Energy Adoption: 
A Data-Driven Analysis of Causal and Predictive Patterns Using Authoritative Sources. 
Master's Thesis, IU International University of Applied Sciences.
```

---

## License

This work is available for academic and educational purposes. For commercial use, please contact the author.

---

## Contact

**LinkedIn:** https://www.linkedin.com/in/sunainamanjunath/

---

## Acknowledgments

Thesis completed under the supervision of Prof. Dr. Uma Santhosh Tumpala at IU International University of Applied Sciences.

Data sources: IRENA, World Bank, REN21, Energy Institute
```
