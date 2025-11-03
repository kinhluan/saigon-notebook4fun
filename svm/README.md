# Support Vector Machines

Classic SVM on classic Iris. Maximum margin, minimum fuss.

## What's Inside

- **SVM Kernels**: Linear, RBF, Polynomial
- **Hyperparameter Tuning**: GridSearchCV for C and gamma
- **Evaluation**: Confusion matrix, ROC curves, classification report
- **Visualizations**: Decision boundaries, support vectors, PCA projections
- **Model Comparison**: SVM vs KNN vs Decision Tree vs Random Forest vs Naive Bayes

## Quick Start

Open `SVM_Iris_Colab.ipynb` in Google Colab and run all cells. Watch SVMs draw decision boundaries.

## The Gist

SVMs find the hyperplane that maximizes margin between classes. Support vectors are the critical points that define this boundary.

**RBF Kernel** typically wins (~95-98% accuracy) by handling non-linear patterns.

## Key Features

- **Data Exploration**: Pairplots, correlation heatmaps, class distributions
- **Grid Search**: Automatic C and gamma optimization
- **5-Fold CV**: Robust performance estimates
- **Decision Boundaries**: 2D visualizations with support vectors highlighted
- **ROC Curves**: One-vs-Rest for multiclass classification

## Results Preview

Top performers on Iris:

1. SVM (RBF): ~96%
2. KNN (k=7): ~93%
3. Logistic Regression: ~91%

---

**Author**: Luân B
