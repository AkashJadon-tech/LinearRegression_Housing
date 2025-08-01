# 🏠 Linear Regression on Housing Prices Dataset

This project implements *Linear Regression from scratch using Python and NumPy* to predict house prices based on various features such as area, number of bedrooms, location proximity, and furnishing status.

---

## 📌 Dataset

- *Source*: [Kaggle - Housing Prices Dataset](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset)
- Contains features like:
  - Area (in sq. ft.)
  - Bedrooms
  - Bathrooms
  - Stories
  - Furnishing status
  - Proximity to main road
  - and more

---

## 🛠 What I Did

### ✅ Implemented from Scratch:
- compute_cost with *L2 Regularization*
- compute_gradient
- gradient_descent

### ✅ Data Preprocessing:
- One-hot encoding of categorical variables
- Outlier removal using quantile-based filtering
- Manual and Scikit-learn-based feature scaling
- Train/Test split

### ✅ Model Evaluation:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- RMSE as a % of average price

---

## 📈 Final Results

| Metric               | Value      |
|----------------------|------------|
| Test MSE             | ~1063.28   |
| Test RMSE            | ~1031.15   |
| R² Score             | 0.7227     |
| RMSE % of Avg Price  | ~21.11%    |

> 📌 The model performs reasonably well considering it was implemented *completely from scratch* with regularization and proper scaling.

---

## 🔍 Comparison: Manual vs Scikit-learn Linear Regression

After implementing the model manually, I compared it directly with Scikit-learn’s LinearRegression using the *same preprocessed data*.

| Metric         | Manual              | Scikit-learn         | Difference |
|----------------|---------------------|-----------------------|------------|
| Test MSE       | 1061285782422.56    | 1060142763640.15      | ~0.11%     |
| Test RMSE      | 1030187.25          | 1029632.33            | ~0.05%     |
| R² Score       | 0.7232              | 0.7235                | ~0.03%     |
| Intercept (b)  | 4635731.28          | 4635931.42            | Negligible |
| Weights (w)    | Very close          | Very close            | Minor float diff |

> ✅ The results match *very closely*, proving that the from-scratch implementation is mathematically correct and consistent with sklearn's backend, which uses a more stable SVD-based solution.

## 🚀 How to Run

1. *Clone the repository:*
   ```bash
   git clone https://github.com/AkashJadon-tech/LinearRegression_Housing.git
   cd LinearRegression_Housing
  ---

## 📦 Requirements

Make sure the following libraries are installed:

```bash
numpy
pandas
scikit-learn
matplotlib
seaborn
