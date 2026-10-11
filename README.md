# COVID-19 Data Exploration and Analysis

This project explores COVID-19 case trends using public datasets from Johns Hopkins CSSE, Google mobility reports, and related derived data. The notebooks move from global country-level comparisons to U.S. state-level analysis, including visualizations, rate calculations, mobility comparisons, and introductory forecasting models.

## Project Overview

The project is organized around two Jupyter notebooks:

- `Covid19DataExplorationAndAnalysis_Brennan.ipynb` analyzes global COVID-19 trends. It loads confirmed, deaths, and recovered time-series data; compares countries; calculates worldwide totals, recovery rates, and mortality rates; visualizes country rankings and case growth; and experiments with simple regression-based forecasting.
- `US_specific.ipynb` focuses on U.S. state-level trends. It combines Johns Hopkins U.S. time-series and daily report data with Google mobility data to examine confirmed cases, deaths, recoveries, active cases, incident rates, mortality rates, hospitalization rates, testing rates, mobility changes, growth factors, rolling averages, and state-level forecasting.

## File Structure

- `Covid19DataExplorationAndAnalysis_Brennan.ipynb` - main global COVID-19 exploration notebook.
- `US_specific.ipynb` - U.S.-specific state analysis notebook.
- `complete_covid_data.csv` - derived U.S. state-level dataset with state, coordinates, date, confirmed cases, population, deaths, incidence rate, and mortality rate.
- `README.md` - project overview and summary.

## Main Conclusions

The global notebook shows that by the late-June 2020 snapshot used in the analysis, worldwide confirmed cases exceeded 10 million, reported deaths were just above 500,000, recoveries were about 5.1 million, and active cases were about 4.5 million. The worldwide recovery rate was roughly 50.7%, while the mortality rate was roughly 4.9%.

Country-level comparisons show that COVID-19 impact was highly uneven. Top-10 rankings, log-scale plots, per-capita comparisons, and country-specific views help compare countries with different population sizes and outbreak timing. The U.S. appears as a major case-study country because it had one of the highest confirmed-case totals in the data snapshot.

The U.S.-specific notebook shows that state totals need context from rates and severity indicators. Confirmed cases, deaths, active cases, incident rate, mortality rate, hospitalization rate, and testing rate together provide a clearer picture than raw case counts alone. New York is used repeatedly as an early high-impact example, while the notebook's helper functions allow similar analysis for other states.

Mobility analysis provides another layer of context. Comparing retail, recreation, grocery, transit, and workplace mobility changes against case and severity metrics helps explore how behavior shifted during the pandemic, though these relationships should be interpreted cautiously because they are influenced by testing access, reporting delays, policy decisions, and local conditions.

The regression and Prophet forecasting examples demonstrate how time-series methods can be applied to COVID-19 data, but they are intentionally exploratory. Reliable forecasting would require stronger model validation, more explanatory variables, and careful treatment of changing public-health policy, reporting practices, and behavioral responses.
