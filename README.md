# 🏥 HealthCare-Premium-Prediction

An **Insurance Premium Cost Predictor** built with **Streamlit** and **Machine Learning**.  
The app estimates insurance premiums based on demographics, lifestyle choices, BMI, smoking habits, income, genetic risk, and medical history using pre-trained ML models.

---

## 🚀 Overview

This project combines a **Streamlit frontend** with a **scikit-learn + XGBoost backend** to predict healthcare premiums.  
The pipeline includes preprocessing, scaling, and risk scoring to ensure accurate predictions for different demographic groups.

---

## 📂 Project Structure

HealthCare-Premium-Prediction/
│
├── app/ # Streamlit application
│ ├── main.py # Web app entry point
│ └── prediction_helper.py # Helper functions for predictions
│
├── artifacts/ # Pre-trained models & scalers
│ ├── model_rest.joblib
│ ├── model_young.joblib
│ ├── scaler_rest.joblib
│ └── scaler_young.joblib
│
├── Model_training_and_all_resources/ # Data & training notebooks
│ ├── Data_segmentation.ipynb
│ ├── ml_premium_prediction.ipynb
│ ├── ml_premium_prediction_rest.ipynb
│ ├── ml_premium_prediction_rest_with_gr.ipynb
│ ├── ml_premium_prediction_young.ipynb
│ ├── ml_premium_prediction_young_with_gr.ipynb
│ ├── premiums.xlsx
│ ├── premiums_rest.xlsx
│ ├── premiums_young.xlsx
│ ├── premiums_rest_with_gr.xlsx
│ └── premiums_young_with_gr.xlsx
│
├── .gitignore
├── LICENSE # Apache-2.0 license
├── README.md # Project documentation
└── requirements.txt # Python dependencies

yaml
Copy code

---

## ⚙️ Installation & Usage

### 1. Prerequisites
- Python **3.x**
- Recommended: Create a virtual environment

### 2. Setup
```bash
git clone https://github.com/Arun-Hegde/HealthCare-Premium-Prediction.git
cd HealthCare-Premium-Prediction
pip install -r requirements.txt
Key libraries:
joblib, pandas, numpy, streamlit, scikit-learn, xgboost

3. Run the Application
bash
Copy code
cd app
streamlit run main.py
Your browser will open with the Health Insurance Cost Predictor.

🛠️ Technologies Used
Frontend: Streamlit

Backend: Python, scikit-learn, XGBoost

Data Processing: Pandas, NumPy

Model Serialization: Joblib

🌟 Future Enhancements
🔹 Add more features for robust predictions

🔹 User authentication system

🔹 Detailed breakdown of premium calculation

🔹 Cloud deployment (AWS, Azure, GCP)

📜 License
This project is licensed under the Apache 2.0 License
