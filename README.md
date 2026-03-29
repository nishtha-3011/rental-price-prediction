# 🏠 RentIQ — AI Rental Price Predictor

A machine learning web application that predicts Airbnb rental prices 
using XGBoost, trained on real Airbnb listing data.

---

## 🌐 Live Demo
[Click here to open the website](https://nishtha-3011.github.io/rental-price-prediction/rental_prediction_website.html)

---

## 📌 Features

- 🤖 XGBoost ML model with 94%+ accuracy
- 🏙️ Covers 10 major US metropolitan cities
- 🏠 Predicts based on 10 real features
- 🔐 User login & registration system
- 📜 Prediction history saved per user
- 🌙 Beautiful dark-themed responsive UI

---

## 🎯 Input Features Used for Prediction

| Feature | Description |
|--------|-------------|
| City | Metropolitan city (NY, LA, SF, etc.) |
| Property Type | Apartment, Villa, House, Loft, etc. |
| Room Type | Entire home / Private room / Shared room |
| Bed Type | Real Bed, Futon, Sofa, etc. |
| Cancellation Policy | Flexible / Moderate / Strict |
| Accommodates | Number of guests |
| Bedrooms | Number of bedrooms |
| Bathrooms | Number of bathrooms |
| Beds | Number of beds |
| Minimum Nights | Minimum stay required |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| ML Model | XGBoost, Scikit-learn |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, SHAP |
| Frontend | HTML, CSS, JavaScript |
| Notebook | Jupyter Notebook |

---

## 📁 Project Structure
```
rental-price-prediction/
│
├── airbnb_price_prediction.ipynb   ← ML pipeline (XGBoost)
├── rental_prediction_website.html  ← Frontend website
├── README.md                       ← You are here
└── model_artifacts/                ← Generated after running notebook
    ├── xgb_price_model.pkl
    ├── le_room.pkl
    ├── le_neigh.pkl
    ├── le_neigh_grp.pkl
    └── model_metadata.json
```

---

## ▶️ How to Run

### 1. ML Model (Jupyter Notebook)
```bash
# Install libraries
pip install xgboost scikit-learn pandas numpy matplotlib seaborn joblib shap

# Open Jupyter
jupyter notebook

# Open airbnb_price_prediction.ipynb
# Click Kernel → Restart & Run All
```

### 2. Website (Frontend)
```bash
# No server needed! Just double click:
rental_prediction_website.html
```

---

## 📊 ML Workflow
```
Data Loading → EDA → Cleaning → Feature Engineering
      ↓
Model Comparison (Linear, Ridge, RF, GBM, XGBoost)
      ↓
XGBoost Hyperparameter Tuning (GridSearchCV)
      ↓
Evaluation (MAE, RMSE, R², SHAP)
      ↓
Save Model Artifacts
```

---

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| Model | XGBoost |
| R² Score | 0.9420 |
| MAE | ~$18/night |
| RMSE | ~$28/night |

---

##  Dataset

[Airbnb Price Prediction — Kaggle](https://www.kaggle.com/datasets/stevezhenghp/airbnb-price-prediction)

---

##  Author

Made with  using XGBoost + HTML/CSS/JS
