# Strategic Insights through Advanced Data Analysis  
**Enhancing Business Performance with Statistical Modeling and Machine Learning Techniques**  
**Author**: Suriya Subbiah Perumal  

---

## 📌 Overview

This project presents a comprehensive multi-phase analysis of a large business dataset to uncover strategic insights. It integrates data cleaning, imputation, exploratory analysis, and advanced predictive modeling to support decision-making.

---

## 🧾 Project Workflow

### 1. **Initial Data Filtering**
- Focused on high-frequency categories to ensure statistical robustness and relevance.
- Hypothesis-driven filtering improved the interpretability of insights.

### 2. **Data Quality Comparison**
- Compared the original dataset with a cleaned version (excluding `0`s and `NA`s).
- Explored the impact of data quality on analysis outcomes.

### 3. **Missing Data Imputation**
- Applied **PCA** (for numerical features) and **k-NN** (for categorical features).
- Ensured data integrity for modeling by using sophisticated imputation techniques.

---

## 📊 Statistical Modeling Techniques

### 🔹 Lasso Regression
- Used for feature selection and to identify influential predictors from large variable sets.

### 🔹 Generalized Additive Models (GAM)
- Applied to understand non-linear relationships between variables and target outcomes.

### 🔹 Support Vector Machines (SVM)
- Deployed for classification and regression tasks to enhance predictive accuracy.
- Model performance assessed using multiple evaluation metrics.

---

## 📈 Visualization Strategy

- Comprehensive plots were used to interpret data transformations and modeling outcomes.
- Visual diagnostics supported model validation and interpretation.

---

## 🧪 Tools and Libraries

- **Data Preparation**: `dplyr`, `fastDummies`, `missMDA`, `VIM`, `readr`
- **Modeling**: `glmnet`, `mgcv`, `e1071`, `caret`, `Metrics`
- **Visualization**: `ggplot2`, `DT`, `scales`, `reshape2`
- **Reporting**: `gt`, `knitr`, `kableExtra`

---

## 🔍 Key Insights

- Cleaning and imputing missing data significantly enhanced data usability.
- Lasso helped in reducing model complexity without sacrificing performance.
- GAM revealed non-linear patterns crucial for understanding business dynamics.
- SVM models performed well in both classification and prediction tasks, offering a robust solution for business forecasting.

---

## 📌 Conclusion

This project demonstrates the value of combining statistical rigor with machine learning techniques for business intelligence. By leveraging both imputation and predictive modeling, it is possible to derive actionable insights even from imperfect datasets.

---



