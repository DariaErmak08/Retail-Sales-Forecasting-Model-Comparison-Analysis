# 🛍️ Retail Sales Forecasting: Model Comparison & Analysis

This project is focused on building and evaluating multiple machine learning models to forecast daily sales across retail stores. Using time-series data, promotional metadata, and calendar information, we train and compare the performance of various algorithms.

---

## 📌 Project Goals
- Predict daily sales for retail stores based on historical data
- Evaluate different ML models and select the best-performing one
- Analyze prediction errors and uncover improvement opportunities

---

## 📁 Dataset
The dataset includes:
- **Sales records** with store-wise daily transaction information
- **Promotional flags** and holidays
- **Features** such as day of week, month, and special promo periods

---

## ⚙️ Preprocessing Steps
- Date parsing and time-based feature engineering
- Categorical encoding of promo types and state holidays
- Handling of missing values
- Train/test split

---

## 🤖 Models Evaluated
- ✅ **LightGBM** (Best RMSE: 1759.14)
- 🔶 **XGBoost** (RMSE: 1822.36)
- 🟦 **CatBoost** (RMSE: 2204.13)
- 🌲 **Random Forest** (Train RMSE: 338.62)

---

## 📈 Visualizations & Insights
- 📊 *Actual vs Predicted Sales*: High alignment with minimal variance
- 📉 *Prediction Error Distribution*: Errors mostly within ±2000 range
- 🗓 *Absolute Error by Day of Week*: Higher error on weekends
- 📢 *Error by Promo*: No-promo days showed unexpected outliers
- 🏪 *Top 20 Stores by Avg. Error*: A few stores consistently underperform
- 📅 *Error by Month*: Some months show irregular outliers

---

## 📋 Recommendations
- Integrate external factors (weather, holidays, events)
- Use store-specific modeling for high-error stores
- Improve promo feature granularity
- Deploy LightGBM as a baseline production model

---

## 🛠 Tech Stack
- **Languages:** Python
- **Libraries:** pandas, scikit-learn, LightGBM, XGBoost, CatBoost, matplotlib, seaborn
- **IDE:** Jupyter Notebook

---

## 📂 Folder Structure

```
retail-sales-forecasting/
│
├── data/                  # Raw and cleaned data files
├── notebooks/             # Jupyter notebooks with EDA & model training
├── models/                # (Optional) Saved models for reuse
├── visualizations/        # PNGs or charts for README/reporting
├── requirements.txt       # Required Python libraries
└── README.md              # Project documentation
```

---

## 📧 Contact
For questions, collaborations or feedback, please reach out via GitHub Issues or email.
