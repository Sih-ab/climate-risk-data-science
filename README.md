# Climate Risk Data Science: Dhaka, Bangladesh

## Overview
This project analyzes historical climate data for Dhaka, Bangladesh, from 1981 to 2025. It examines long-term trends in temperature, relative humidity, and rainfall using Python.

## Objectives
- Analyze historical climate patterns.
- Investigate long-term climate trends.
- Apply statistical methods to identify trends.
- Explore potential implications for climate risk assessment.

## Dataset
- **Source:** NASA POWER
- **Location:** Dhaka, Bangladesh
- **Period:** 1981–2025
- **Frequency:** Daily
- **Variables:**
  - `T2M`: Daily near-surface air temperature (°C)
  - `RH2M`: Relative humidity at 2 meters (%)
  - `PRECTOTCORR`: Corrected precipitation (mm/day)

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- pymannkendall
- Jupyter Notebook

## Methodology
1. Load and clean climate data.
2. Validate dates and missing values.
3. Calculate annual and monthly climate summaries.
4. Visualize historical climate patterns.
5. Apply the Mann–Kendall trend test.
6. Estimate trend slopes using Sen's slope.
7. Export processed data and statistical results.

## Preliminary Findings
The analysis of the NASA POWER dataset indicates:

- Annual mean temperature has a statistically significant decreasing trend.
- Annual mean relative humidity has a statistically significant increasing trend.
- Annual total precipitation has a statistically significant increasing trend.

These are preliminary findings from the selected dataset and analysis period. Independent observations and additional statistical checks are needed before drawing conclusions about actual climate change.

## Conclusion

This project analyzed daily NASA POWER climate data for Dhaka, Bangladesh, from 1981 to 2025. The dataset contained 16,436 daily records, with no missing values in the selected temperature, relative humidity, and precipitation variables.

The Mann–Kendall trend analysis identified the following patterns:

- Annual mean temperature showed a statistically significant decreasing trend.
- Annual mean relative humidity showed a statistically significant increasing trend.
- Annual total precipitation showed a statistically significant increasing trend.
- The number of zero-rainfall days showed a decreasing trend.
- The number of heavy-rainfall days (daily precipitation ≥ 50 mm) showed an increasing trend.

These results suggest changes in the distribution of rainfall and humidity in the selected NASA POWER dataset. However, they should be interpreted cautiously. Independent weather observations, data-quality checks, and statistical methods that account for temporal autocorrelation are needed to validate the findings.

This project demonstrates how Python-based data analysis and non-parametric statistical methods can be used to investigate historical climate patterns and support further climate-risk research.

## Project Structure
```text
climate-risk-data-science/
├── data/
│   └── processed/
│       ├── climate_data_cleaned.csv
│       └── climate_trend_summary.csv
├── notebooks/
│   └── climate_risk_analysis.ipynb
└── README.md