# 📈 Demand Forecasting System

Machine Learning project to predict product demand using pricing, discounts, promotions, inventory, and competitor pricing data.

Includes a Streamlit web application for real-time demand prediction.

---

## 🚀 Features

- Predict product demand
- Real-time Streamlit app
- XGBoost Regressor model
- Hyperparameter tuning using RandomizedSearchCV
- Feature importance analysis

---

## 📁 Dataset

Dataset: `demand_forecasting.csv`

### Features
- Price
- Discount
- Inventory Level
- Promotion
- Competitor Pricing
- Category

### Target
- Demand

---

## 🤖 Model Used

- XGBoost Regressor

### Best Parameters

```python
{
 'subsample': 1.0,
 'n_estimators': 300,
 'min_child_weight': 3,
 'max_depth': 6,
 'learning_rate': 0.1,
 'colsample_bytree': 1.0
}
```

---

## 📊 Model Performance

- RMSE: **35.55**

---

## 📈 Feature Importance

| Feature | Importance |
|---------|------------|
| Promotion | 0.566 |
| Category | 0.267 |
| Price | 0.092 |
| Competitor Pricing | 0.031 |
| Discount | 0.025 |
| Inventory Level | 0.019 |

### Key Insight
Promotion and Category have the highest impact on product demand.

---

## 💻 Streamlit App

Users can:
- Enter product details
- Predict product demand instantly

---

## ▶️ Run Project

### Install Requirements

```bash
pip install -r requirements.txt
```

### Run App

```bash
streamlit run app.py
```

---

## 📦 Files

- app.py
- xgboost_demand_model.pkl
- label_encoders.pkl
- Demand Forecasting.ipynb
- demand_forecasting.csv

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Streamlit

---


## 👨‍💻 Author

**Ram Vilas**  
Data Science & AI Enthusiast  

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
