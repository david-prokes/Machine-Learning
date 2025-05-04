# Wage Model Validation (R)

This project applies regression modeling and cross-validation techniques to analyze wage determinants based on education, seniority, and gender. The analysis is based on the 2022 Spanish Survey of Wage Structure (EES).

## Objective

To identify and quantify key factors influencing salary using polynomial regression models and to evaluate their performance using k-fold and leave-one-out cross-validation (LOOCV).

## Methodology

- **Data preparation**: Filtering, transformations, and factor encoding.
- **Exploratory analysis**: Visualization of wage distributions by gender and education.
- **Modeling**:
  - Polynomial regression (degrees 1 to 5)
  - Interaction effects (gender × seniority)
  - Model selection based on cross-validation MSE
- **Evaluation**: Comparison of models with/without interaction terms.

## Key Findings

- Gender pay gap: Women earn ~29.7% less, controlling for other variables.
- Seniority has a nonlinear impact on wages.
- Educational level correlates positively with earnings.
- The effect of seniority varies significantly between genders.

## Tools

- **Language**: R  
- **Libraries**: `dplyr`, `ggplot2`, `boot`, `here`