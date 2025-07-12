# 🔢 Sales Forecasting in Python

Simple sales prediction model I built using Random Forest. Nothing fancy, just straight to the point.

### 💡 What it does

- I cleaned and processed the data (converted week into day/month/year)
- Removed outliers (top 1% of sales units)
- Encoded store_id and sku_id using one-hot
- Compared 3 models: RandomForest, Ridge, and GradientBoosting
- RandomForest gave the best RMSE, so I tuned it a bit and used it
- Final model is trained and used to predict on `test.csv`

### 🛠️ Tech used

- Python
- pandas / scikit-learn
- RandomForestRegressor
- Pipeline + ColumnTransformer

### 📁 Files

- `train.csv` — base training data
- `test.csv` — test data to make predictions on
- `test_predictions.csv` — final output file

### 🚀 How to run

Make sure you have `train.csv` and `test.csv` in the same folder.

```bash
pip install -r requirements.txt
python model_train.py
