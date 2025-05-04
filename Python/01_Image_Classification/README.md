# CIFAR-10 Image Classification (Python)

This project classifies images from a reduced version of the CIFAR-10 dataset using supervised learning algorithms such as SVM, KNN, Random Forest, and AdaBoost.

## Objective

To classify low-resolution color images from three randomly selected categories and compare the performance of different classifiers using cross-validation.

## Methodology

- Loading and combining binary batches of CIFAR-10 image data.  
- Each image represented by 3072 pixel features (RGB channels).  
- Random selection of 3 categories from 10 possible labels.  
- Dimensionality analysis through color intensity distribution.  
- Model evaluation using 5-fold cross-validation.  
- Comparison of SVM (linear & RBF), KNN (weighted), Random Forest, and AdaBoost.

## Key Findings

- SVM with RBF kernel achieved the best performance (~75% accuracy).  
- Logistic SVM reached 71% accuracy but struggled with one class.  
- KNN performed poorly overall but showed strength on one specific class.  
- Visual features alone are not sufficient for high-accuracy classification across all categories.

## Tools

**Language:** Python  
**Libraries:** `numpy`, `matplotlib`, `scikit-learn`, `pickle`, `pandas`