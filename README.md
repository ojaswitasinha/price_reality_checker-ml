# Price Reality Checker 💻💰

A machine learning project that predicts laptop prices from their specifications. It compares regression models and shows how closely their predictions match actual prices.

---

## 📌 Project Overview

This project uses laptop features such as brand, processor, RAM, storage, graphics, screen size, operating system, and weight to predict a laptop’s listed price.

The notebook trains and evaluates regression models, then displays actual prices alongside predictions and residuals.

---

## 🔧 Techniques Used

- Data inspection and preprocessing
- Missing-value imputation
- One-hot encoding for categorical features
- Train/test split
- Median baseline
- Linear Regression
- Random Forest Regression
- MAE, RMSE, and R² evaluation
- Actual-versus-predicted price comparison
- Residual analysis

---

## 📂 Files in This Repo

- `price_reality_checker.ipynb` — Notebook for loading the dataset, training models, and reviewing predictions
- `laptop_price.csv` - Laptop Price Dataset
- `README.md` — Project documentation

---

## 🚀 How to Run

### 1. Clone the repo
```bash
git clone https://github.com/ojaswitasinha/price_reality_checker-ml.git
cd price-reality-checker-ml
```

### 2. Install dependencies
```
pip install scikit-learn pandas numpy
```

---

## 🧠 Model Evaluation

The notebook compares these regressors:

- **Median baseline** — predicts the median price from the training data
- **Linear Regression** — estimates price using a weighted combination of laptop features
- **Random Forest Regressor** — combines decision trees to learn more complex patterns

Performance is measured using:

- **MAE** — average absolute prediction error
- **RMSE** — prediction error that gives larger errors more weight
- **R²** — proportion of price variation explained by the model

Add the measured scores here after running the notebook. No results are included until the models have been evaluated.

---

## 📊 Residuals

A residual is the difference between an actual price and its predicted price:

```text
Residual = Actual Price - Predicted Price
```

A positive residual means the actual price is higher than predicted. A negative residual means it is lower. Large residuals may be useful for finding listings to investigate, but do not by themselves prove that a price is unusual.

---

## ✨ Future Improvements

- Flag listings with unusually large prediction errors
- Add a form for entering laptop specifications and receiving a price estimate
- Tune model parameters and compare additional regression models
- Add charts for actual versus predicted prices
