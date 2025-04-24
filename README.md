# Strategic Business Insights Through Advanced Data Analysis  
**Suriya Subbiah Perumal**  


---

## 📌 Introduction

This project presents a multi-phase analytical approach to uncover insights from business datasets to enhance decision-making. From data cleaning to predictive modeling, this report delivers actionable strategies using robust statistical techniques.

---

## 🧾 Data Filtering & Preparation

- Focused on frequent categories: field_cat values of 18, 21, 45, 58, 59.
- Resulting dataset: **4280 rows × 21 columns**.
- Cleaned version (no NAs/zeros): **402 rows**.
- PCA used for numerical imputation; KNN for categorical imputation.

---

## 🛠 Data Transformation

- Created dummy variables for `score`.
- Converted other categorical columns to factors for simplicity and computational efficiency.

---

## 📊 Visualizations Summary

1. **Bar Chart**: Claim distribution across U.S. states — PA & TN had high business concentrations.
2. **Histogram**: Review counts skewed right; most businesses had < 50 reviews.
3. **Density Plot**: Total claim services revealed a multimodal distribution.
4. **Scatter Plot**: Branded vs Generic claim services showed a strong positive correlation.
5. **Violin Plot**: CEO graduation years varied by gender; female CEOs peaked in mid-2000s.
6. **Box Plot**: Review score distributions by state — FL and NJ performed slightly better.
7. **Scatter Plot**: Review counts vs scores by state — slight negative correlation noted.

---

## 🔍 Subsetting & Lasso Regression

Subsets created based on `field_cat` values. Each subset underwent Lasso Regression to select key predictors.

- **Subset 1**: Top variables included `Rural_metropolitan_Desc`, `city`, `CEO_grd_yr`
- **Subset 2–4**: Predictors like `postal_code`, `review_count`, `business_id` emerged as significant

---

## 📈 Generalized Additive Models (GAM)

Performance varied across subsets:
| Model | Accuracy | Precision | Recall | F1 Score | AUC |
|-------|----------|-----------|--------|----------|-----|
| GAM-1 | 50.3%    | 48.8%     | 48.1%  | 48.4%    | 0.55|
| GAM-3 | 60.3%    | 57.6%     | 59.4%  | 58.5%    | 0.60|

---

## 🤖 Support Vector Machines (SVM)

SVM outperformed GAMs, especially in recall:

- **SVM-2 to SVM-4** had **100% recall** but lower precision (~57%)
- Accuracy remained steady across subsets (~58.5%)

> 🔍 **SVM selected as best model** due to high recall — ideal for high-stakes classification problems.

---

## ✅ Conclusion

- Imputation methods (PCA, KNN) preserved dataset integrity
- Lasso identified strong predictors across regions and business features
- SVM demonstrated robustness in identifying all positive cases, making it the preferred model

---

## 📚 Tools Used

- R (`caret`, `glmnet`, `mgcv`, `e1071`)
- PCA & KNN for imputation
- ggplot2 for visualization

---

## 📌 Recommendations

- Fine-tune SVM kernel and cost parameters for better precision
- Consider interaction effects and non-linear terms in future models
- Use model insights for regional business strategy and customer engagement plans
