# HealthCare-Premium-Prediction

🏥 Health Insurance Cost Predictor using Machine Learning.

-----

## Overview

This project is an insurance premium cost predictor built using a **Streamlit** front end and a **scikit-learn** back end. It estimates insurance premiums based on a comprehensive set of factors, including demographics, lifestyle choices, income, BMI, smoking habits, genetic risk, and medical history. The machine learning pipeline includes preprocessing, scaling, and a risk-scoring mechanism to provide accurate predictions.

-----

## Project Structure

The repository is organized into the following directories and files:

  * **`app/`**: Contains the Streamlit application code.

      * `main.py`: The main file for the Streamlit web application.
      * `prediction_helper.py`: A helper script for managing prediction logic and functions.

  * **`artifacts/`**: Stores the pre-trained machine learning models and scalers.

      * `model_rest.joblib`: The trained model for a specific demographic group (e.g., non-young adults).
      * `model_young.joblib`: The trained model for the "young" demographic group.
      * `scaler_rest.joblib`: The scaler object corresponding to the `model_rest.joblib`.
      * `scaler_young.joblib`: The scaler object corresponding to the `model_young.joblib`.

  * **`Model_training_and_all_resources/`**: Houses the data and Jupyter notebooks used for model training and experimentation.

      * `Data_segmentation.ipynb`: Notebook for data exploration and segmentation.
      * `ml_premium_prediction.ipynb`: Main notebook for training the base machine learning model.
      * `ml_premium_prediction_rest.ipynb`: Notebook for training the model for the "rest" demographic.
      * `ml_premium_prediction_rest_with_gr.ipynb`: Notebook for the "rest" model including genetic risk.
      * `ml_premium_prediction_young.ipynb`: Notebook for training the "young" demographic model.
      * `ml_premium_prediction_young_with_gr.ipynb`: Notebook for the "young" model including genetic risk.
      * `premiums.xlsx`, `premiums_rest.xlsx`, `premiums_young.xlsx`, `premiums_rest_with_gr.xlsx`, `premiums_young_with_gr.xlsx`: Datasets used for model training.

  * **`.gitignore`**: Specifies files and directories to be excluded from version control.

  * **`LICENSE`**: The project's license (Apache-2.0).

  * **`README.md`**: This readme file.

  * **`requirements.txt`**: Lists all Python dependencies required to run the project.

-----

## Installation and Usage

To run this project, you'll need to install the required Python packages and run the Streamlit application.

### Prerequisites

Make sure you have **Python 3.x** installed.

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/Arun-Hegde/HealthCare-Premium-Prediction.git
    cd HealthCare-Premium-Prediction
    ```
2.  Install the required libraries using `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```
    The key libraries include `joblib`, `pandas`, `streamlit`, `numpy`, `scikit-learn`, and `xgboost`.

### Running the Application

Once the dependencies are installed, you can launch the Streamlit app from the `app` directory.

```bash
cd app
streamlit run main.py
```

This will start a local server and open the web application in your default browser.

-----

## Technologies Used

  * **Frontend**: Streamlit
  * **Backend**: Python, scikit-learn, XGBoost
  * **Data Manipulation**: Pandas, NumPy
  * **Model Serialization**: Joblib

-----

## Future Enhancements

  * Add more features for a more robust model.
  * Integrate a user authentication system.
  * Provide a detailed breakdown of the premium calculation.
  * Deploy the application to a cloud service like AWS, Azure, or GCP.
