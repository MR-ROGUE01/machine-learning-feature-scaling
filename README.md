# Standardization & Model Performance Analysis

This project explores the practical impact of Standardization in Machine Learning using Python and Scikit-learn. The goal of this notebook was not only to apply feature scaling but also to understand how different machine learning algorithms behave before and after standardization.

Using `StandardScaler`, I transformed the feature distributions and compared model performance through visualization and regression analysis.

---

## Project Workflow

* Data Preprocessing & Exploration
* Train-Test Split
* Standardization using StandardScaler
* Scatter Plot Visualization
* KDE Distribution Analysis
* Linear Regression
* KNN Regression
* Performance Evaluation using R² Score

---

## Key Findings

### Linear Regression

Linear Regression performance remained almost unchanged after standardization because the algorithm is largely scale-invariant and focuses on learning linear relationships between variables.

### KNN Regression

KNN Regression showed a major improvement after scaling:

* **Before Standardization:** 0.8496
* **After Standardization:** 0.9839

This improvement occurred because KNN is a distance-based algorithm. Standardization balanced the contribution of all features and improved distance calculations significantly.

---

## Visualizations Included

* Before vs After Scaling Scatter Plots
* KDE Distribution Plots
* Feature Distribution Comparison

These visualizations helped in understanding how feature distributions changed after standardization and how scaling impacts data representation.

---

## Technologies Used

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn • Jupyter Notebook

---

## Conclusion

This project helped me build a deeper understanding of preprocessing techniques in Machine Learning, especially the practical importance of Standardization for distance-based algorithms.

It also strengthened my understanding of:

* Feature Scaling
* Data Visualization
* Regression Analysis
* Model Evaluation
* Algorithm Behavior before and after preprocessing

The project focuses on learning through implementation, experimentation, and visual interpretation rather than only theoretical understanding.
