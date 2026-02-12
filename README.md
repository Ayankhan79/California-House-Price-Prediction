## 🏠 House Price Prediction (California Housing Dataset)

### 📌 Project Overview

This project focuses on predicting **median house prices** using the **California Housing Dataset**.
Multiple regression models were trained and evaluated to understand how well different algorithms capture the relationship between housing features and prices.

The goal was to **compare linear vs tree-based models** and identify the best-performing approach using proper evaluation metrics.

---

### 🧠 Models Implemented

* **Linear Regression**
* **Lasso Regression**
* **Random Forest Regressor**
* **XGBoost Regressor**

---

### 📊 Evaluation Metrics

Models were evaluated on both **training** and **test** datasets using:

* **R-squared (R²)** – goodness of fit
* **Mean Absolute Error (MAE)** – average prediction error

---

### 📈 Model Performance Comparison

| Model                   | Train R² | Train MAE |    Test R² |   Test MAE |
| ----------------------- | -------: | --------: | ---------: | ---------: |
| **XGBoost Regressor**   |   0.9468 |    0.1876 | **0.8365** | **0.3066** |
| Random Forest Regressor |   0.9733 |    0.1218 |     0.8101 |     0.3259 |
| Linear Regression       |   0.6074 |    0.5299 |     0.6010 |     0.5367 |
| Lasso Regression        |   0.2817 |    0.7662 |     0.2825 |     0.7819 |

---

### 🏆 Best Performing Model

**XGBoost Regressor** emerged as the best model:

* Highest **Test R²: 0.8365**
* Lowest **Test MAE: 0.3066**
* Strong generalization compared to Random Forest

This indicates XGBoost effectively captures **complex non-linear relationships** present in housing data while avoiding overfitting.

---

### ⚠️ Least Effective Models

* **Lasso Regression**

  * Test R²: 0.2825
  * High MAE indicates poor predictive capability
  * Linear model with L1 regularization struggled with non-linearity
* **Linear Regression**

  * Moderate performance (Test R² ≈ 0.60)
  * Unable to model complex feature interactions

---

### 🔍 Key Insights

* Tree-based models (**XGBoost, Random Forest**) significantly outperform linear models.
* Housing prices depend on **non-linear interactions** between features.
* Regular linear models are insufficient for this dataset.

---

### 🚀 Future Improvements

* Hyperparameter tuning for XGBoost
* Feature importance analysis
* Error analysis on high-priced and low-priced regions

---
