Figures and Visualizations

This folder contains all key visualizations and outputs from the Master's thesis analysis on global renewable energy adoption (2000-2023).

Overview

Total Figures: 18 
Format: JPG (screenshots from Jupyter Notebook outputs)
Source: Analysis conducted in Python using pandas, statsmodels, scikit-learn, and visualization libraries
Thesis: Modelling and Forecasting Global Renewable Energy Adoption | Sunaina Manjunath | IU International University

Complete Figure List
1. Correlation Matrix
Filename: Correlation Matrix.jpg
Description:
Heatmap showing pairwise correlations between key variables including log GDP per capita, log population, log energy use per capita, electricity access percentage, and total renewable energy capacity. Values range from -1 (perfect negative correlation) to +1 (perfect positive correlation).
Key Insight:
Confirms positive correlations between economic indicators (GDP, population) and renewable capacity. GDP per capita shows strongest correlation with renewable adoption. Energy use shows weaker positive correlation. Used as preliminary multicollinearity check before regression modeling.
Used in: Chapter 4, Section 4.2 (Exploratory Data Analysis)

2. Data & Panel Construction
Filename: Data & Panel Construction.jpg
Description:
Table documenting the structure and composition of the final panel dataset, showing variable names, data types, observation counts, and summary statistics. Displays the cleaned and harmonized dataset used for all analytical procedures.
Key Insight:
Documents the final dataset structure: 211 countries × 24 years = 5,064 observations. Shows complete variable coverage after data cleaning and imputation procedures. Demonstrates data quality and readiness for econometric analysis.
Used in: Chapter 3 (Methodology) and Chapter 4, Section 4.1 (Overview of Analytical Pipeline)

3. Descriptive Statistics Output
Filename: Descriptive Statistics Output.jpg
Description:
Summary statistics table displaying count, mean, median, standard deviation, minimum, and maximum values for all continuous variables in the dataset, including solar PV capacity, onshore wind capacity, offshore wind capacity, total renewable capacity, GDP per capita, population, electricity access, and energy use per capita.
Key Insight:
Mean renewable capacity significantly exceeds median, revealing heavily right-skewed distribution. A few countries dominate global capacity while most remain at low levels. This skewness justified logarithmic transformations applied in regression analysis. Shows data spans from near-zero capacity to over 1 million MW.
Used in: Chapter 4, Section 4.2 (Descriptive and Exploratory Results)

4. Economic Development and Renewable Energy Adoption
Filename: Economic Development and Renewable Energy Adoption.jpg
Description:
Scatter plot showing relationship between log GDP per capita (x-axis) and total renewable energy capacity in megawatts (y-axis) across all countries and years in the panel dataset. Each point represents a country-year observation.
Key Insight:
Clear positive correlation between economic development and renewable adoption. Higher-income countries consistently show higher capacity levels, supporting regression findings that GDP is a primary driver. Visual evidence of the wealth-capacity relationship before formal econometric testing.
Used in: Chapter 4, Section 4.2 (Exploratory Data Analysis)

5. FE vs RE Comparison Table
Filename: FE vs RE comparison table.jpg
Description:
Side-by-side comparison table of Fixed Effects and Random Effects panel regression model outputs, including coefficient estimates, standard errors, R-squared values (within, between, overall), F-statistics, and Hausman test results.
Key Insight:
Hausman test p-value below 0.05 confirms Fixed Effects is the statistically appropriate specification for this dataset. Country-specific unobserved effects are correlated with explanatory variables, violating Random Effects assumptions. Validates Fixed Effects as main econometric model.
Used in: Chapter 4, Section 4.3 (Econometric Results - Model Selection)

6. Fixed Effects Summary
Filename: Fixed Effects summary.jpg
Description:
Complete regression output table for Fixed Effects panel model with clustered standard errors, showing coefficient estimates, robust standard errors, t-statistics, p-values, confidence intervals, within R-squared (0.4716), F-statistics, and model diagnostics for all explanatory variables.
Key Insight:
Main econometric model controlling for time-invariant country characteristics. All key predictors (GDP per capita, population, electricity access) are statistically significant at p<0.001 level. Within R-squared of 0.47 indicates model explains 47% of within-country variation over time. Energy use shows negative coefficient, suggesting fossil fuel dependency creates inertia.
Used in: Chapter 4, Section 4.3 (Main Econometric Results)

7. Forecast Accuracy Table
Filename: Forecast Accuracy Table.jpg
Description:
Performance comparison table showing Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE) for three forecasting models (ARIMA, Prophet, XGBoost) across three countries (Germany, India, USA).
Key Insight:
ARIMA demonstrates most consistent performance across all three countries with lowest average error rates. Prophet performs well for non-linear growth patterns (India). XGBoost shows higher variance and occasional overfitting. No single model dominates everywhere—context and country characteristics matter. MAPE ranges from 0.2% (excellent) to 16% (poor).
Used in: Chapter 4, Section 4.4 (Forecasting Results - Performance Evaluation)

8. Forecast Comparison - Germany
Filename: Forecast Comparison - Germany.jpg
Description:
Time-series visualization comparing actual renewable energy capacity (observed values) against predictions from ARIMA, Prophet, and XGBoost models for Germany from 2000-2023. Shows historical trend and forecast trajectories with confidence intervals where applicable.
Key Insight:
ARIMA tracks Germany's smooth, stable growth trend most accurately. Prophet slightly overshoots but captures trend well. XGBoost visibly underfits, showing limitations on stable, predictable time series. Germany represents a mature, developed renewable energy market with consistent policy support.
Used in: Chapter 4, Section 4.4 (Forecasting Results)

9. Forecast Comparison - India
Filename: Forecast Comparison - India.jpg
Description:
Forecast comparison plot for India showing rapid, non-linear capacity growth and model predictions. Displays actual values versus ARIMA, Prophet, and XGBoost forecasts over the 2000-2023 period.
Key Insight:
Prophet performs best for India's accelerating, non-linear growth pattern. ARIMA underestimates due to assuming linear trends. India represents an emerging economy with rapid renewable expansion driven by recent policy initiatives and falling technology costs. Demonstrates context-specific model performance.
Used in: Chapter 4, Section 4.4 (Forecasting Results)

10. Forecast Comparison - USA
Filename: Forecast Comparison - USA.jpg
Description:
USA renewable capacity forecasts comparing actual observed values with predictions from all three forecasting models (ARIMA, Prophet, XGBoost) across the full time period.
Key Insight:
Intermediate case between Germany's stability and India's volatility. ARIMA remains most consistent performer. XGBoost shows highest forecast error. USA represents large, diverse energy market with mixed state-level policies creating moderate growth trajectory.
Used in: Chapter 4, Section 4.4 (Forecasting Results)

11. Global Renewable Energy Capacity Trends
Filename: Global Renewable Energy Capacity Trends.jpg
Description:
Multi-line time-series chart showing global installed renewable electricity capacity from 2000-2023, disaggregated by technology type (solar PV, onshore wind, offshore wind) and total renewable capacity. Y-axis shows capacity in megawatts, x-axis shows years.
Key Insight:
Demonstrates steep acceleration in renewable deployment after 2010, driven primarily by solar PV which shows exponential growth. Onshore wind shows steady linear growth. Offshore wind remains smallest but growing. Total global capacity increased over 20-fold during study period, with most growth concentrated post-2010 when technology costs declined sharply.
Used in: Chapter 4, Section 4.2 (Descriptive and Exploratory Results)

12. Global Trends Table Output
Filename: Global Trends Table Output.jpg
Description:
Year-by-year numerical table showing global installed capacity totals for solar PV, onshore wind, offshore wind, and total renewable electricity capacity from 2000-2023. Provides exact megawatt figures underlying the trends visualization.
Key Insight:
Quantifies the magnitude of renewable growth. Solar PV increased from approximately 1,000 MW in 2000 to over 1,000,000 MW by 2023—a roughly 1,000-fold increase in 24 years. Wind capacity also showed multi-fold growth. Numerical data supports visual trend analysis.
Used in: Chapter 4, Section 4.2 (Descriptive Results)

13. Pooled OLS Summary
Filename: Pooled OLS summary.jpg
Description:
Regression output table for Pooled Ordinary Least Squares model showing coefficient estimates, HC3 robust standard errors, z-values, p-values, 95% confidence intervals, R-squared (0.595), F-statistic, AIC, BIC, and diagnostic statistics. Treats all observations as independent without accounting for panel structure.
Key Insight:
Baseline specification ignoring country-level heterogeneity. R-squared of 0.595 appears reasonable but poolability F-test strongly rejects this model in favor of panel estimators. All coefficients significant but estimates are biased due to not controlling for country-specific effects. Shown for methodological comparison, not as primary result.
Used in: Chapter 4, Section 4.3 (Econometric Results - Baseline Comparison)

14. Random Effects Summary
Filename: Random Effects summary.jpg
Description:
Complete regression output for Random Effects panel model showing coefficient estimates, clustered standard errors, t-statistics, p-values, within/between/overall R-squared values, F-statistics, and model diagnostics. Assumes country-specific effects are uncorrelated with regressors.
Key Insight:
Alternative panel specification tested but rejected by Hausman test. Overall R-squared (0.5589) higher than Fixed Effects but this masks failure to properly control for correlation between unobserved effects and predictors. Coefficient estimates differ from Fixed Effects, particularly for population and energy use. Shown for methodological transparency and formal model comparison.
Used in: Chapter 4, Section 4.3 (Econometric Results - Model Comparison)

15. SHAP Dependence Plot
Filename: SHAP dependence plot.jpg
Description:
Scatter plot showing how SHAP (Shapley Additive Explanations) contribution values for GDP per capita vary across its value range. X-axis shows GDP per capita values, y-axis shows corresponding SHAP values (marginal contribution to predictions). Color gradient indicates interaction with population variable.
Key Insight:
Reveals non-linear relationship between GDP and renewable capacity predictions. SHAP contribution accelerates at higher income levels, showing threshold effects that a single linear regression coefficient cannot capture. High GDP countries (pink points) contribute more positively to predictions. Demonstrates value of machine learning in capturing complex relationships beyond linear models.
Used in: Chapter 4, Section 4.5 (Explainability Results) and Chapter 5 (Discussion)

16. SHAP Summary Plot
Filename: SHAP Summary Plot.jpg
Description:
Beeswarm plot ranking all explanatory variables by their absolute SHAP value contributions to XGBoost model predictions. Each dot represents an observation, color indicates feature value (red=high, blue=low), position shows SHAP contribution (positive pushes prediction up, negative down). Variables ordered by importance from top to bottom.
Key Insight:
GDP per capita dominates feature importance by massive margin, far exceeding all other predictors. Energy use per capita shows negative SHAP values (high energy use reduces predicted capacity). Population and electricity access have smaller but positive contributions. Confirms economic development is primary driver even in complex machine learning model, not just in linear regression.
Used in: Chapter 4, Section 4.5 (Explainability Results)

17. Top Countries Output
Filename: Top Countries Output.jpg
Description:
Ranked table listing the top 15 countries by maximum total renewable energy capacity (megawatts) achieved during the 2000-2023 study period. Shows country names and corresponding peak capacity values.
Key Insight:
China leads by enormous margin with over 1 million MW, followed by USA (286,000 MW), Germany (144,000 MW), India (115,000 MW), and Japan (92,000 MW). Demonstrates extreme concentration of global renewable capacity in handful of countries. Top 15 countries account for majority of worldwide installed capacity, highlighting inequality in adoption patterns.
Used in: Chapter 4, Section 4.2 (Descriptive and Exploratory Results)

18. VIF Output
Filename: VIF Output.jpg
Description:
Table showing Variance Inflation Factor (VIF) values for all explanatory variables used in panel regression models. VIF measures degree of multicollinearity—how much each predictor's variance is inflated due to correlation with other predictors.
Key Insight:
All VIF values well below conventional threshold of 5 (except constant, which is not concerning). Log GDP per capita has highest VIF at 3.95 but still acceptable. Confirms no problematic multicollinearity among predictors. Each variable contributes independently to model without excessive correlation issues. Validates regression model stability and reliability of coefficient estimates.
Used in: Chapter 4, Section 4.3 (Econometric Diagnostics)

Organization by Chapter
Chapter 4.2 - Descriptive and Exploratory Analysis

Global Renewable Energy Capacity Trends
Economic Development and Renewable Energy Adoption
Correlation Matrix
Descriptive Statistics Output
Top Countries Output
Global Trends Table Output

Chapter 4.3 - Econometric Modeling

Data & Panel Construction
Pooled OLS Summary
Fixed Effects Summary
Random Effects Summary
FE vs RE Comparison Table
VIF Output

Chapter 4.4 - Forecasting Results

Forecast Comparison - Germany
Forecast Comparison - India
Forecast Comparison - USA
Forecast Accuracy Table

Chapter 4.5 - Explainability Analysis

SHAP Summary Plot
SHAP Dependence Plot


How to Use These Figures
Viewing
All figures are JPG format and can be viewed in any image viewer or browser. Double-click any file to open.
Citing
If using these visualizations, please cite:
Manjunath, S. (2025). Modelling and Forecasting Global Renewable Energy Adoption: 
A Data-Driven Analysis of Causal and Predictive Patterns Using Authoritative Sources. 
Master's Thesis, IU International University of Applied Sciences.
Embedding in Documents
To embed in Markdown (e.g., README.md):
markdown![Figure Title](figures/Filename.jpg)
*Caption: Brief description*
To embed in HTML:
html<img src="figures/Filename.jpg" alt="Figure Title" width="800">
<p><em>Caption: Brief description</em></p>

Regenerating Figures
All figures can be regenerated from the Jupyter Notebook analysis:

Open Sunaina_Thesis_Data_Analysis.ipynb
Run all cells in sequence
Figures are generated as inline outputs
Right-click any figure → Save image as PNG (higher quality than screenshots)

Regenerating ensures figures reflect any updated data or methodology changes.

Technical Details
Image Format: JPG (screenshots)
Recommended Format for Web: PNG (better quality, no compression artifacts)
Typical Resolution: 1920x1080 or higher
Color Space: RGB
Compression: Medium (balance between quality and file size)
Optimization for GitHub:

Current JPG files work well for web display
GitHub automatically optimizes image loading
File sizes under 5MB load quickly


License and Usage
These figures are outputs from academic research conducted for a Master's thesis at IU International University of Applied Sciences.
Permitted Use:

Academic and educational purposes
Personal portfolio and job applications
Research presentations and publications (with citation)

Attribution Required:
Please credit: Sunaina Manjunath, IU International University (2025)
Commercial Use:
Contact author for permissions regarding commercial use.

Contact
For questions about these visualizations or access to underlying data:
Author: Sunaina Manjunath 
Email: sunainamgowda@gmail.com
LinkedIn: www.linkedin.com/in/sunainamanjunath/
GitHub Repository: https://github.com/Sunaina2005/Thesis-Renewable-Energy-Adoption-Data-Analysis

Last Updated: January 2025
