# 🏥 HealthCare-Premium-Prediction

An **Insurance Premium Cost Predictor** built with **Streamlit** and **Machine Learning**.  
This project estimates health insurance premiums by analyzing multiple factors such as demographics, lifestyle choices, BMI, smoking habits, income, genetic risk, and medical history.  

---

## 📖 Table of Contents
- [Overview](#-overview)
- [Project Structure](#-project-structure)
- [Installation & Usage](#️-installation--usage)
- [Technologies Used](#-technologies-used)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## 🚀 Overview
The application combines a **Streamlit frontend** with a **scikit-learn + XGBoost backend** to predict healthcare premiums.  
The ML pipeline includes:
- Data preprocessing & segmentation  
- Feature scaling  
- Risk scoring  
- Separate models for different demographic groups  

This ensures **personalized and accurate premium predictions**.

---

## 📂 Project Structure

```
HealthCare-Premium-Prediction/
│
├── app/ # Streamlit application 
│ ├── main.py # Web app entry point 
│ └── prediction_helper.py # Prediction logic & helpers 
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
├── README.md # Documentation 
└── requirements.txt # Python dependencies 

```
---

## ⚙️ Installation & Usage

### 1. Prerequisites
- Python **3.x**  
- Recommended: Create and activate a virtual environment  

### 2. Clone Repository
```bash
git clone https://github.com/Arun-Hegde/HealthCare-Premium-Prediction.git
cd HealthCare-Premium-Prediction
```

### 3. Install Dependencies

```bash
Copy code
pip install -r requirements.txt
Core libraries:
joblib, pandas, numpy, streamlit, scikit-learn, xgboost
```

### 4. Run the Application
```
bash
Copy code
cd app
streamlit run main.py
Your default browser will open the Health Insurance Cost Predictor app.
```

### 🛠️ Technologies Used

- Frontend: Streamlit

- Backend: Python, scikit-learn, XGBoost

- Data Processing: Pandas, NumPy

- Model Serialization: Joblib
