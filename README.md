# 🔢 Sales Forecasting in Python

Simple notebook that predicts sales units using Random Forest. Nothing overcomplicated , just preprocessing, model training, and prediction. Everything is inside `salesEstimator.ipynb`.

---

### 💡 What it does

- Reads and processes `train.csv` and `test.csv`
- Converts `week` column to day/month/year
- Removes top 1% outliers in `units_sold`
- One-hot encodes `store_id` and `sku_id`
- Compares 3 models: `RandomForest`, `Ridge`, and `GradientBoosting`
- Chooses `RandomForest` based on best RMSE
- Trains final model and makes predictions for `test.csv`
- Outputs predictions as `test_predictions.csv`

---

### 🛠️ Tech used

- Python
- pandas
- scikit-learn
- RandomForestRegressor
- Pipelines (for preprocessing + modeling)

---

### 📁 Files

| File | Description |
|------|-------------|
| `salesEstimator.ipynb` | Full notebook with preprocessing, modeling, and prediction logic |
| `train.csv` | Raw training data |
| `test.csv` | Test set for prediction |
| `test_predictions.csv` | Model's predicted sales units |
| `.gitignore` | Ignores system folders like `.ipynb_checkpoints` |

---

### 🚀 How to run

This project runs as a notebook:

1. Open `salesEstimator.ipynb` in Jupyter or VS Code
2. Run all cells step by step
3. Output file `test_predictions.csv` will be created in the same folder

---

That’s it . clear and compact. 
