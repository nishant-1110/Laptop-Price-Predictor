# Laptop-Price-Predictor

This project predicts the prices of laptops based on various features such as brand, storage (SSD and HDD), screen resolution, weight, and processor type. The goal is to assist users in estimating laptop prices using machine learning models.

## Features
1. Input Features:
Brand, Processor, RAM, Storage (SSD, HDD), Screen Resolution, Weight, GPU, Operating System.
2. Output:
Predicted laptop price.

## Project Overview
1. A machine learning pipeline is implemented to streamline the data preprocessing and modeling steps.
2. The model uses Random Forest Regressor with OneHotEncoding to handle categorical features and numerical feature scaling, ensuring accurate price predictions.

## Workflow
1. Data Preprocessing:
-> Applied One-Hot Encoding to categorical variables like brand and processor.
   
-> Used a ColumnTransformer to apply transformations to selected columns while passing others through unchanged.

3. Model Training:
-> Used Random Forest Regressor with specific hyperparameters (n_estimators=100, max_samples=0.5, max_features=0.75, max_depth=15).
   
-> Fitted the pipeline to training data.

4. Model Evaluation:
-> R² Score: Achieved 89%.
   
-> Mean Absolute Error (MAE): 0.15.

## Key Technologies
1. Python
2. Scikit-learn for machine learning model development
3. Pandas and NumPy for data manipulation
4. Pipeline and ColumnTransformer for efficient data preprocessing
5. RandomForestRegressor for regression modeling

## How to Run the Project
1. Clone the repository:
git clone https://github.com/your-username/laptop-price-predictor.git

2. Install dependencies:
pip install -r requirements.txt

3. Run the project:
streamlit run app.py
