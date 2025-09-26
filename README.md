# 📉 Customer Churn Prediction MVP

Predict which customers are likely to churn (stop using a service) using machine learning, and receive **actionable retention strategies** to reduce revenue loss.

Built with **XGBoost**, **Plotly**, and **Gradio** — ready to run in **Google Colab** or locally.


---

## 🎯 Model Summary

> “An Model churn-prediction system that takes customer data, predicts who is likely to churn, and visualizes high-risk segments so the business can take proactive retention measures.”

- **Accuracy**: ~82%  
- **AUC**: ~0.87  
- **Output**: Churn probability + retention strategy per customer  
- **Tools**: Python, Scikit-learn, XGBoost, Plotly, Gradio

---

## 📦 Features

✅ **Smart Preprocessing**  
- Handles missing `TotalCharges`  
- Encodes categorical variables (One-Hot + Label)  
- Scales numeric features  

✅ **High-Performance Model**  
- Hyperparameter-tuned XGBoost classifier  
- Optimized decision threshold (0.4 instead of 0.5)  

✅ **Actionable Insights**  
- Retention strategy recommendations (e.g., *"Offer 1-year contract + $10 discount"*)  
- High-risk customer export (`high_risk_customers.csv`)  

✅ **Interactive Visualizations**  
- Top churn drivers (feature importance)  
- Churn probability distribution  
- Precision-recall vs threshold analysis  

✅ **Real-Time Prediction**  
- Gradio web app for instant scoring  
- Public demo link (when deployed)

---

## 🚀 Quick Start (Google Colab)

1. Open the notebook:  https://colab.research.google.com/drive/1o0x1ADrnnqOn7FIhyAkudGfpsZzUkOA8?usp=sharing

2. Run all cells — it will:
   - Train the model
   - Show interactive charts
   - Launch a **Gradio web app** (click the public link!)

> 💡 No setup needed — runs entirely in the browser.

---

## 📁 Project Structure
customer-churn-prediction/
├── churn_prediction_mvp.ipynb # Main Colab notebook (recommended)
├── churn_prediction_mvp.py # Standalone script version
├── churn_model.pkl # Trained model (joblib)
├── model_info.json # Metadata (threshold, features)
├── high_risk_customers.csv # Sample output of at-risk customers
└── README.md # You are here!
