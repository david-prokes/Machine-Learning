# Governance Clustering & PCA (R)

This project analyzes governance indicators from the Worldwide Governance Indicators (WGI) dataset using Principal Component Analysis and K-means clustering.

## Objective
To reduce the dimensionality of governance data and classify countries into clusters based on institutional quality.

## Methodology
- PCA to capture the main axes of variance among six governance indicators.
- Optimal number of components selected based on the explained variance (85.5% with PC1, 92% with PC2).
- K-means clustering applied to the principal components, choosing k=3 as a meaningful trade-off.
- Interpretation of clusters as developed, developing, and underdeveloped governance profiles.

## Key Findings
- Two principal components capture most of the variation.
- Three clusters reflect broad global governance typologies.
- PCA helps summarize complex institutional data in a meaningful way.

## Tools
- **Language**: R  
- **Libraries**: `readxl`, `dplyr`, `ggplot2`, `tidyr`, `reshape2`