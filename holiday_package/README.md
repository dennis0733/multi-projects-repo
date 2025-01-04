# Holiday Package Analysis/Prediction

This project analyzes customer data from "Trips & Travel.Com" to predict potential customers for a new Wellness Tourism package. The goal is to improve marketing efficiency by targeting the most likely customers.

## About the Dataset

The dataset includes information about past customers and their travel package purchases. It covers a period of [Data Time Period] and contains various features that might influence package selection.

### Context

"Trips & Travel.Com" currently offers five package types: Basic, Standard, Deluxe, Super Deluxe, and King. However, customer acquisition costs were high due to random marketing approaches. The company aims to leverage customer data for targeted marketing of the new Wellness Tourism package.

### Content

The dataset includes features such as:

* Designation (e.g., Executive, Manager)
* Passport (Yes/No)
* Tier City (Tier 1, Tier 2, Tier 3)
* Marital Status (Married/Single)
* Occupation
* Monthly Income
* Age
* Preferred Hotel Star Rating (e.g., 3-star, 5-star)
* Package Purchased (Yes/No)

## Project Structure

The project is organized into the following folders:

holiday_package_analysis/ ├── data/ │ ├── raw_data.csv # Original dataset │ └── cleaned_data.csv # Processed dataset ├── notebooks/ │ ├── eda.ipynb # Exploratory data analysis │ └── model_training.ipynb # Model development and evaluation ├── models/ │ ├── random_forest.pkl # Trained Random Forest model │ ├── logistic_regression.pkl # Trained Logistic Regression model │ └── scaler.pkl # Data preprocessor ├── reports/ │ ├── eda_report.html # Automated EDA report │ └── performance_report.html # Model evaluation report ├── scripts/ │ ├── preprocess.py # Data preprocessing script │ └── train_model.py # Model training script └── README.md # Project documentation

## Analysis and Modeling

This project involves the following steps:

1. **Exploratory Data Analysis (EDA):**
    * Understanding data distribution and relationships between features.
    * Identifying key features that influence package selection.
    * Data cleaning and preprocessing.

2. **Model Training:**
    * Training and evaluating different machine learning models (Logistic Regression, Decision Tree, Random Forest) to predict potential customers for the Wellness Tourism package.
    * Hyperparameter tuning to optimize model performance.

3. **Model Selection:**
    * Selecting the best performing model based on evaluation metrics.

## Inspiration

This project aims to:

* Analyze customer data to understand travel preferences.
* Recommend marketing strategies to target potential customers for the new package.
* Build a predictive model to identify customers likely to purchase the Wellness Tourism package.

This project provides valuable insights for "Trips & Travel.Com" to optimize marketing campaigns and increase sales of the new travel package.
