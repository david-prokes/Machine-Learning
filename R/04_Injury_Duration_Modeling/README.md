# Injury Duration Prediction – Regression & Variable Selection (R)
*Econometrics Final Paper*

This project explores the duration of workers' compensation claims (`ldurat`) using the `injury` dataset from Wooldridge’s econometrics data collection. The goal is to predict `ldurat` using classical and penalized regression techniques, comparing model performance and variable selection methods.

## Objectives

- Estimate and interpret linear models using socioeconomic and medical variables.
- Apply best subset selection and forward selection with cross-validation.
- Evaluate Ridge, LASSO, Principal Component Regression (PCR), and Partial Least Squares (PLS).
- Compare prediction error and model interpretability.

## Methodology

- Linear regression and log-log interpretations
- Multicollinearity diagnosis via VIF
- Best subset and forward stepwise selection (with k-fold CV)
- Ridge & LASSO regression with lambda tuning
- Principal Component Regression (PCR)
- Partial Least Squares (PLS)
- Model evaluation with MSE and CV error

## Key Findings

- Benefit amount, age, hospitalization, and total medical cost are significant predictors.
- All selection methods (subset, forward) converge on a 4-variable model.
- LASSO shrinks irrelevant coefficients to zero and selects 10–12 variables depending on CV folds.
- PCR yields the lowest test error (1.18), with 18 components retained.
- PLS is slightly less accurate but more parsimonious (3 components).