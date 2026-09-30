# Waze User Churn — Exploratory Data Analysis

## Project Overview
This project explores Waze user behaviour to identify patterns associated with churn. The analysis examines app usage, driving activity, tenure, device type, distance, driving duration, activity days and driving days.

## Business Problem
Understanding how retained and churned users differ can help identify behavioural signals for retention analysis and later predictive modelling.

## Objectives
- Inspect the dataset and assess data quality.
- Explore distributions, skewness and potential outliers.
- Compare retained and churned users across behavioural measures.
- Engineer additional features for deeper analysis.
- Translate analytical findings into business recommendations.

## Tools and Technologies
- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset
The analysis uses `waze_dataset.csv`, containing user-level behavioural and engagement measures together with a churn/retention label.

## Analytical Workflow
1. Load and inspect the dataset.
2. Review data types, descriptive statistics and missing information.
3. Explore sessions, drives, tenure, distance, driving duration, activity days and driving days.
4. Examine device and churn distributions.
5. Compare behavioural patterns across retained and churned users.
6. Engineer behavioural features, including kilometres driven per driving day and recent-session measures.
7. Investigate and manage extreme numerical values.
8. Summarise findings, recommendations and limitations.

## Selected Results
- The overall churn rate is approximately 17%.
- Churn proportions are broadly similar across iPhone and Android users.
- Sessions, drives, distance and driving duration are strongly right-skewed and contain high-value observations.
- Activity days and driving days provide useful measures of engagement.
- Lower recent engagement is associated with higher churn in this dataset.
- Some distance-per-driving-day and recent-session values require further validation because of unusually large or inconsistent observations.

## Business Recommendations
- Prioritise behavioural engagement variables when investigating churn.
- Avoid making device-specific retention decisions from this exploratory analysis alone.
- Investigate low-activity users as a potential retention segment.
- Validate extreme behavioural values before predictive modelling.
- Use the EDA findings to guide subsequent statistical testing and feature selection.

## Limitations
This is exploratory analysis. Observed relationships are associations and should not be interpreted as causal effects. Extreme and unusual values require validation before modelling.

## Repository Contents
- `waze_exploratory_data_analysis.ipynb` — complete analysis notebook
- `waze_dataset.csv` — project dataset
- `README.md` — project documentation

## How to Run
1. Clone or download the repository.
2. Install the required Python libraries.
3. Open `waze_exploratory_data_analysis.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the notebook cells from top to bottom.

## Next Steps
The EDA provides a foundation for formal statistical testing and predictive churn modelling.
