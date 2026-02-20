Data Sources
This document provides direct links and instructions for obtaining all datasets used in the thesis analysis.

Primary Data Sources
1. IRENA Renewable Capacity Statistics
Source: International Renewable Energy Agency (IRENA)
Access: https://pxweb.irena.org/pxweb/en/IRENASTAT
What you need:

Dataset: "Electricity Capacity and Generation"
Technologies: Solar photovoltaic, Onshore wind energy, Offshore wind energy
Time period: 2000-2023
Coverage: All countries
Grid connection: On-grid only

Download Instructions:

Go to the IRENA Statistics portal
Navigate to "Query" → "Electricity Capacity and Generation"
Select "Installed Capacity" from the data type dropdown
Choose technologies: Solar PV, Onshore Wind, Offshore Wind
Select all countries and years 2000-2023
Select "On-grid" connection type only
Export as CSV

Expected filename: IRENA_Electricity_Installed_Capacity_Solar_PV_Wind_2000_2023.csv

2. World Bank World Development Indicators (WDI)
Source: The World Bank Group
Access: https://databank.worldbank.org/source/world-development-indicators
Required Indicators:

GDP per capita (current US$) - Code: NY.GDP.PCAP.CD
Population, total - Code: SP.POP.TOTL
Access to electricity (% of population) - Code: EG.ELC.ACCS.ZS
Energy use (kg of oil equivalent per capita) - Code: EG.USE.PCAP.KG.OE

Download Instructions:

Go to World Bank DataBank
Select "World Development Indicators" database
Click "Country" → Select all countries
Click "Series" → Search and select the 4 indicators above
Click "Time" → Select years 2000-2023
Click "Download Options" → Choose CSV format
Download the file

Expected filename: WorldBank_WDI_Core_Indicators_2000_2023.csv

3. REN21 Renewables in Cities Global Status Report
Source: REN21 (Renewable Energy Policy Network for the 21st Century)
Access: https://www.ren21.net/reports/global-status-report/
What you need:

Report: Renewables in Cities 2021 Global Status Report
Specifically: Reference Tables (R1-R6) from the Data Pack

Download Instructions:

Visit REN21 Reports page
Find "Renewables in Cities 2021 Global Status Report"
Download the accompanying "Data Pack" (Excel file)
Use Tables R1-R5 for policy indicators:

R1: Renewable Energy Targets
R2: Electric Vehicle Targets
R3-R5: Policy frameworks by country



Expected filename: REC_2021_Datapack.xlsx
Note: This file contains city-level and national renewable energy policy data. For the thesis, national-level policy presence indicators were extracted and coded as binary variables.

4. Energy Institute Statistical Review of World Energy
Source: Energy Institute (formerly BP Statistical Review)
Access: https://www.energyinst.org/statistical-review
What you need:

Full dataset: 2025 Statistical Review of World Energy
Focus sheets:

Solar Installed Capacity
Wind Installed Capacity
Renewable Power Generation
Total Energy Supply



Download Instructions:

Go to Energy Institute website
Navigate to "Statistical Review" section
Download the complete Excel workbook (usually released annually in June)
File contains ~100 sheets - you'll primarily use renewable energy sheets

Expected filename: EI-Stats-Review-ALL-data.xlsx
Note: This dataset was used for cross-validation and robustness checks, confirming consistency with IRENA capacity data.

Data Processing Notes
Time Period
All datasets cover 2000-2023 (24 years)
Geographic Coverage

Started with: 224 countries/territories
Final analysis: 211 countries
Excluded: 13 countries with >40% missing data on core variables

Variable Transformations Applied

Log transformations: GDP per capita, population, energy use per capita, renewable capacity
Interpolation: Linear interpolation for gaps ≤2 consecutive years
Standardization: All variables standardized (mean=0, std=1) for clustering analysis

Missing Data Treatment

Maximum 40% missingness threshold for country inclusion
Conservative interpolation (limit=2 consecutive years)
Imputation flags created for all filled values
CO₂ emissions dropped due to excessive missingness (>60%)


File Organization in Analysis
Once downloaded, organize files as:
data/
├── IRENA_Electricity_Installed_Capacity_Solar_PV_Wind_2000_2023.csv
├── WorldBank_WDI_Core_Indicators_2000_2023.csv
├── REC_2021_Datapack.xlsx
└── EI-Stats-Review-ALL-data.xlsx

Data Licensing & Attribution
IRENA: Open access under Creative Commons Attribution license (CC BY 4.0)
World Bank: Open data with no restrictions on use
REN21: Available for non-commercial use with attribution
Energy Institute: Available for academic and non-commercial use
Citation Requirements:
When using this data, cite:

IRENA (2024). Renewable Capacity Statistics 2024. International Renewable Energy Agency.
World Bank (2024). World Development Indicators. The World Bank Group.
REN21 (2021). Renewables in Cities 2021 Global Status Report. Paris: REN21 Secretariat.
Energy Institute (2025). Statistical Review of World Energy 2025.


Data Quality Notes
Strengths:

Authoritative sources with global coverage
Consistent methodology across countries
Annual updates ensuring current data
Publicly verifiable and reproducible

Limitations:

National-level aggregation (subnational variation hidden)
Reporting quality varies by country income level
Policy data less granular than capacity data
Some early-year data (2000-2005) has more gaps


Alternative Data Sources (Not Used)
These sources were considered but not used in final analysis:

Our World in Data: Aggregates from primary sources above, adds minimal value
IEA Statistics: Paywall restrictions, less comprehensive renewable breakdown
National energy agencies: Inconsistent reporting standards across countries
Ember Climate: Excellent for electricity generation but limited capacity data


Questions?
If you have trouble accessing any datasets or need clarification on data processing steps, refer to Chapter 3 (Methodology) of the thesis document.
Last Updated: January 2025
