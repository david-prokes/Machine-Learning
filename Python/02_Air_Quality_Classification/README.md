# Air Quality Classification – Hospital Joan March (Python)

This project classifies air quality levels based on hourly pollutant and meteorological data collected at the Hospital Joan March monitoring station between 2002 and 2018.

## Objective

To define a custom air quality index using threshold-based logic from official reports, and train supervised learning models capable of classifying air quality conditions without knowing explicit pollutant limits.

## Methodology

- Data loading and exploratory analysis on 16 environmental variables.
- Definition of the target variable ("air quality") based on hourly thresholds from the Balearic Islands’ official air quality report.
- Data cleaning, resampling and rebalancing of quality categories.
- Model training with:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - AdaBoost
- Evaluation via cross-validation and classification metrics (accuracy, confusion matrix).

## Key Findings

- Variables such as NO₂, PM₁₀, and O₃ are key drivers in air quality classification.
- Random Forest showed the best performance in distinguishing moderate and poor quality levels.
- AdaBoost improved minority class prediction despite class imbalance.
- The model was able to learn pollutant interactions without direct access to regulatory thresholds.

## Tools

**Language:** Python  
**Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `imblearn`