# 💼 Salary Dataset — Feature Scaling with StandardScaler + ML Comparison

A hands-on machine learning project demonstrating **feature scaling using StandardScaler** on a Salary dataset, along with a comparison of model performance (Linear Regression & KNN) before and after scaling.

---

## 📁 Dataset

**File:** `Salary_Data.csv`

| Column | Description |
|--------|-------------|
| `Age` | Age of the employee |
| `Salary` | Annual salary |
| `YearsExperience` | Years of work experience *(target variable)* |

---

## 📌 Project Workflow

### 1. Data Loading & Inspection
- Load `Salary_Data.csv` using `pandas`
- Check shape, data types, null values, and duplicates

### 2. Train-Test Split
- Target: `YearsExperience`
- Features: `Age`, `Salary`
- Split: **80% train / 20% test** with `random_state=42`

### 3. Feature Scaling — StandardScaler
- Fit scaler **only on training data** (prevents data leakage)
- Transform both train and test sets
- Converts features to **mean = 0, std = 1**

### 4. Visualizations
- **Scatter plots** — Age vs Salary before and after scaling
- **KDE plots** — Combined Age & Salary distributions
- **KDE plots** — Individual feature distributions (Age, Salary) before vs. after

### 5. Model Comparison — With & Without Scaling

| Model | Before Scaling (R²) | After Scaling (R²) |
|-------|--------------------|--------------------|
| Linear Regression | — | — |
| KNN Regressor (k=3) | — | — |

> 💡 Fill in your R² scores above after running the script!

---

## 📊 Key Observations from Plots

### KDE Plots (Before vs After Scaling)
- Before scaling, `Age` (~20–60) and `Salary` (~10k–150k) live on completely different scales
- After StandardScaler, both features are centered around **0** with comparable spread

### Scatter Plots (Before vs After Scaling)
- The **shape and structure** of the data is preserved
- Only the axis scale changes — relative distances between points remain the same

---

## 💡 Why Scaling Matters

- **Linear Regression** — coefficients are not affected by scale, so R² stays similar
- **KNN Regressor** — heavily distance-based; scaling significantly improves performance because features with larger ranges dominate distance calculations without scaling

---

## 🛠️ Tech Stack

- Python 3.x
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/MR-ROGUE01/machine-learning-feature-scaling.git
cd machine-learning-feature-scaling
```

### 2. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 3. Add the dataset

Place `Salary_Data.csv` in the root of the project directory.

### 4. Run the script

```bash
python salary_scaling.py
```

---

## 📂 Project Structure

```
machine-learning-feature-scaling/
│
├── salary_scaling.py       # Main script
├── Salary_Data.csv         # Dataset
├── README.md               # Project documentation
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
