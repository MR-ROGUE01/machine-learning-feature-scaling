# Feature Scaling & Model Performance Analysis

This project explores the impact of Feature Scaling on different Machine Learning algorithms using Python and Scikit-learn.

The notebook focuses on understanding how scaling affects model behavior, feature distribution, and prediction performance through practical implementation and visualization.

---

## Workflow

* Data Preprocessing
* Train-Test Split
* Feature Scaling using StandardScaler
* Scatter Plot & KDE Visualization
* Linear Regression
* KNN Regression
* Model Evaluation using R² Score

---

## Key Observations

### Linear Regression

Linear Regression performance remained almost unchanged after scaling because the algorithm is mostly scale-invariant.

### KNN Regression

KNN showed significant improvement after applying feature scaling:

* Before Scaling: **0.8496**
* After Scaling: **0.9839**

This happened because KNN is highly dependent on distance calculations, and scaling balanced the contribution of all input features.

---

## Visualizations Included

* Before vs After Scaling Scatter Plots
* KDE Distribution Plots
* Feature Distribution Comparison

---

## Technologies Used

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn • Jupyter Notebook

---

## Conclusion

This project helped me understand the practical importance of Feature Scaling and how different machine learning algorithms react differently to standardized data. It also improved my understanding of preprocessing, visualization, and model evaluation techniques in Machine Learning.
