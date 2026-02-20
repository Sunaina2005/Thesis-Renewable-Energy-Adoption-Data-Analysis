Figures and Visualizations
This document describes all key visualizations from the thesis analysis. Upload your screenshot images to the figures/ folder in your repository.

How to Use These Figures

Extract your Screenshots.zip file
Upload all .jpg files to a new figures/ folder in your GitHub repo
These figures can be embedded in your main README or viewed here


List of Figures
1. Global Renewable Energy Capacity Trends
Filename: Global Renewable Energy Capacity Trends.jpg
Description: Time-series visualization showing the growth of global renewable electricity capacity from 2000-2023, broken down by technology type (solar PV, onshore wind, offshore wind, and total renewable capacity).
Key Insight: Demonstrates the steep acceleration in renewable deployment after 2010, driven primarily by solar PV. Shows the non-linear growth pattern that traditional forecasting models struggle to capture.
Used in: Chapter 4, Section 4.2 (Descriptive and Exploratory Results)

2. Economic Development and Renewable Energy Adoption
Filename: Economic Development and Renewable Energy Adoption.jpg
Description: Scatter plot showing the relationship between log GDP per capita (x-axis) and total renewable capacity in MW (y-axis) across all countries and years.
Key Insight: Clear positive correlation between economic development and renewable adoption. Higher-income countries consistently show higher capacity levels, supporting the econometric regression findings.
Used in: Chapter 4, Section 4.2 (Exploratory Analysis)

3. Correlation Matrix
Filename: Correlation Matrix.jpg
Description: Heatmap showing pairwise correlations between key variables: log GDP per capita, log population, log energy use, electricity access percentage, and total renewable capacity.
Key Insight: Confirms positive correlations between economic indicators and renewable capacity. Used as preliminary multicollinearity check before regression modeling.
Used in: Chapter 4, Section 4.2 (Exploratory Analysis)

4. Descriptive Statistics Output
Filename: Descriptive Statistics Output.jpg
Description: Summary statistics table (count, mean, median, std dev, min, max) for all continuous variables in the final dataset.
Key Insight: Mean renewable capacity is significantly higher than median, revealing right-skewed distribution and justifying log transformations. Shows data quality across 5,064 observations.
Used in: Chapter 4, Section 4.2

5. Top Countries Output
Filename: Top Countries Output.jpg
Description: Table ranking the top 15 countries by maximum total renewable energy capacity (MW) observed during 2000-2023.
Key Insight: China leads by a massive margin, followed by USA, Germany, India, and Japan. Demonstrates the concentration of renewable capacity in a small number of countries.
Used in: Chapter 4, Section 4.2

6. Data & Panel Construction
Filename: Data & Panel Construction.jpg
Description: Table showing the structure of the final panel dataset including variables, observation counts, and data types.
Key Insight: Documents the cleaned dataset used for all analysis: 211 countries × 24 years = 5,064 observations with complete variable coverage.
Used in: Chapter 3 (Methodology) and Chapter 4

7. Pooled OLS Summary
Filename: Pooled OLS summary.jpg
Description: Regression output table for Pooled Ordinary Least Squares model showing coefficients, standard errors, t-statistics, p-values, R-squared, and model diagnostics.
Key Insight: Baseline model ignoring country heterogeneity. R-squared of 0.595 but poolability F-test rejects this specification in favor of panel models.
Used in: Chapter 4, Section 4.3 (Econometric Results)

8. Fixed Effects Summary
Filename: Fixed Effects summary.jpg
Description: Regression output for Fixed Effects panel model with clustered standard errors. Shows within-R-squared of 0.4716 and robust coefficient estimates.
Key Insight: Main econometric model. Controls for country-specific time-invariant factors. All key predictors (GDP, population, electricity access) significant at p<0.001.
Used in: Chapter 4, Section 4.3 (Main Results)

9. Random Effects Summary
Filename: Random Effects summary.jpg
Description: Regression output for Random Effects model showing coefficients and standard errors under the assumption of uncorrelated random effects.
Key Insight: Alternative specification tested but rejected by Hausman test. Shown for methodological transparency and comparison.
Used in: Chapter 4, Section 4.3

10. FE vs RE Comparison Table
Filename: FE vs RE comparison table.jpg
Description: Side-by-side comparison of Fixed Effects and Random Effects model outputs, including Hausman test results.
Key Insight: Hausman test p-value <0.05 confirms Fixed Effects is the appropriate specification. Validates model choice statistically.
Used in: Chapter 4, Section 4.3 (Model Selection)

11. VIF Output
Filename: VIF Output.jpg
Description: Variance Inflation Factor (VIF) values for all predictor variables in the regression models.
Key Insight: All VIF values below 5, confirming no problematic multicollinearity. Each predictor contributes independently to the model.
Used in: Chapter 4, Section 4.3 (Diagnostics)

12. Forecast Comparison - Germany
Filename: Forecast Comparison - Germany.jpg
Description: Time-series plot comparing actual renewable capacity vs. predictions from ARIMA, Prophet, and XGBoost models for Germany (2000-2023).
Key Insight: ARIMA tracks the smooth growth trend most accurately. Prophet slightly overshoots. XGBoost underfits, showing limitations on stable time series.
Used in: Chapter 4, Section 4.4 (Forecasting Results)

13. Forecast Comparison - India
Filename: Forecast Comparison - India.jpg
Description: Forecast comparison plot for India showing rapid, non-linear capacity growth and model predictions.
Key Insight: Prophet performs best for India's accelerating growth pattern. ARIMA underestimates. Demonstrates context-specific model performance.
Used in: Chapter 4, Section 4.4

14. Forecast Comparison - USA
Filename: Forecast Comparison - USA.jpg
Description: USA renewable capacity forecasts from all three models compared to observed values.
Key Insight: Intermediate case between Germany's stability and India's volatility. ARIMA again most consistent, XGBoost shows highest error.
Used in: Chapter 4, Section 4.4

15. Forecast Accuracy Table
Filename: Forecast Accuracy Table.jpg
Description: Table showing RMSE, MAE, and MAPE values for ARIMA, Prophet, and XGBoost across Germany, India, and USA.
Key Insight: ARIMA has lowest average error across countries. No single model dominates everywhere. Context matters more than model complexity.
Used in: Chapter 4, Section 4.4 (Performance Evaluation)

16. Global Trends Table Output
Filename: Global Trends Table Output.jpg
Description: Year-by-year table showing global installed capacity totals for solar PV, onshore wind, offshore wind, and total renewables (2000-2023).
Key Insight: Numerical data behind the trends chart. Solar grows from ~1,000 MW to over 1,000,000 MW—a 1,000-fold increase in 24 years.
Used in: Chapter 4, Section 4.2

17. SHAP Summary Plot
Filename: SHAP Summary Plot.jpg
Description: Beeswarm plot showing SHAP value distributions for each predictor variable in the XGBoost model, ranked by importance.
Key Insight: GDP per capita dominates feature importance by a massive margin. Energy use has negative contribution. Confirms economic drivers also dominate ML predictions.
Used in: Chapter 4, Section 4.5 (Explainability Results)

18. SHAP Dependence Plot
Filename: SHAP dependence plot.jpg
Description: Scatter plot showing how SHAP contributions for GDP per capita vary across its value range, colored by population interaction.
Key Insight: Reveals non-linear relationship—GDP's effect accelerates at higher income levels. Shows threshold effects that linear regression coefficients miss.
Used in: Chapter 4, Section 4.5 and Chapter 5 (Discussion)

Figure Organization
By Chapter:
Chapter 4.2 - Descriptive Analysis:

Global Renewable Energy Capacity Trends
Economic Development and Renewable Energy Adoption
Correlation Matrix
Descriptive Statistics Output
Top Countries Output
Global Trends Table Output

Chapter 4.3 - Econometric Models:

Data & Panel Construction
Pooled OLS Summary
Fixed Effects Summary
Random Effects Summary
FE vs RE Comparison Table
VIF Output

Chapter 4.4 - Forecasting:

Forecast Comparison - Germany
Forecast Comparison - India
Forecast Comparison - USA
Forecast Accuracy Table

Chapter 4.5 - Explainability:

SHAP Summary Plot
SHAP Dependence Plot


How to Embed Figures in README
If you want to show these figures directly in your main README, use this markdown syntax:
![Global Renewable Capacity Trends](figures/Global%20Renewable%20Energy%20Capacity%20Trends.jpg)

*Figure 1: Global renewable electricity capacity growth by technology (2000-2023)*
Note: GitHub will automatically display .jpg and .png images when referenced this way.

Figure File Formats

Current format: JPG (from screenshots)
Recommended for web: Keep as JPG or convert to PNG for higher quality
Size optimization: GitHub handles images well up to ~5MB each


Regenerating Figures
All figures can be regenerated from the Jupyter notebook:

Run Sunaina_Thesis_Data_Analysis.ipynb
Figures are generated in-notebook
Right-click → Save image as .png for higher quality than screenshots


License
These figures are outputs from the thesis analysis and are available for educational and academic use. For commercial use, please contact the author.

Last Updated: January 2025
