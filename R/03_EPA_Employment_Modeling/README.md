# Spanish Labour Market Modeling – EPA 2023 (R)

This project analyzes labour microdata from the Spanish Labour Force Survey (EPA) using various machine learning techniques to model employment status, company seniority, and economic activity classification.

## Objectives

- Predict whether individuals worked during the reference week (binary classification).
- Classify the economic activity (AOI) using LDA and QDA.
- Model company seniority (DCOM) with decision trees, random forest, and boosting.
- Predict future activity sectors (ACT1) with the best-performing model.

## Methodology

- Preprocessing of 43 demographic and work-related variables.
- Binary classification with logistic regression.
- LDA & QDA to classify labour categories with diagnostic tests (Bartlett, M-Box).
- Regression trees, random forests, and boosting for continuous outcomes.
- Variable importance analysis and error comparison.

## Key Findings

- **EDADNum** (age) is the most predictive variable across all models.
- Boosting and Random Forests yield similar MSEs, outperforming simple trees.
- LDA assumptions not met; QDA performs better in discriminant analysis.
- ACT1 prediction explores industry classification for future periods.

## Tools

- **Language**: R  
- **Libraries**: `dplyr`, `ggplot2`, `MASS`, `rpart`, `randomForest`, `gbm`