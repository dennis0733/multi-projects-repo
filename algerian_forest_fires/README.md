Algerian Forest Fires FWI Prediction
This project predicts the Fire Weather Index (FWI) using the Algerian Forest Fires Dataset. The dataset includes environmental and weather-related attributes collected from two regions of Algeria (Bejaia and Sidi Bel-abbes) during the period from June 2012 to September 2012. The project utilizes regression techniques to develop a prediction model and deploys the model as a simple Flask web application.

Dataset Overview
The Algerian Forest Fires Dataset consists of:

Instances: 244 total (122 from Bejaia and 122 from Sidi Bel-abbes).
Attributes:
11 Features: Including Temperature, Relative Humidity, Wind Speed, Rainfall, and others.
1 Target Output: Fire Weather Index (FWI).
Classification Labels:
Fire: 138 instances.
Not Fire: 106 instances.

Dataset Link
https://archive.ics.uci.edu/dataset/547/algerian+forest+fires+dataset

Objective

The goal of this project is to predict the Fire Weather Index (FWI) using various regression models and determine the most effective approach. The models evaluated include:

Linear Regression
Ridge Regression
Lasso Regression
ElasticNet Regression
The best-performing model (Ridge Regression) is then deployed as part of a Flask-based web application.

Project Structure

algerian_forest_fires/
│
├── application.py                # Flask application
├── README.md                     # Project documentation
├── requirements.txt              # Python dependencies
│
├── data/
│   ├── Algerian_forest_fires_dataset_UPDATE.csv  # Original dataset
│   ├── cleaned_dataset.csv                       # Cleaned and processed dataset
│
├── models/
│   ├── ridge.pkl                 # Trained Ridge Regression model
│   ├── scaler.pkl                # StandardScaler for preprocessing
│
├── notebooks/
│   ├── EDA_fires.ipynb           # Exploratory Data Analysis notebook
│   ├── model_training.ipynb      # Model training and evaluation notebook
│
├── templates/
│   ├── index.html                # Web app input form
│   ├── home.html                 # Web app results display



How It Works

Model Training

The dataset is preprocessed to clean and standardize the data.

Multiple regression models are trained and evaluated:

Linear Regression
Ridge Regression
Lasso Regression
ElasticNet Regression

Ridge Regression was selected as the best model based on performance metrics.

Web Application

The Flask framework is used to create a web interface for FWI prediction.
Users can input environmental parameters such as Temperature, Relative Humidity, Wind Speed, Rainfall, and more.
The app uses the trained Ridge Regression model to predict the FWI.

How to Run the Project
1. Clone the Repository
git clone https://github.com/your-username/algerian-forest-fire-prediction.git
cd algerian-forest-fire-prediction

2. Set Up the Environment
Create a virtual environment:

python -m venv venv

Activate the environment:

source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

Install dependencies:

pip install -r requirements.txt

3. Run the Flask App

python application.py
Open a browser and navigate to http://127.0.0.1:5000/ to access the web app.

Example Usage
Open the web app.
Enter values for:
Temperature
Relative Humidity
Wind Speed
Rainfall
Other required parameters.
Click Predict to get the Fire Weather Index (FWI).

Technologies Used

Python: For data preprocessing and model development.
Scikit-Learn: For regression models and preprocessing.
Flask: For building the web application.
HTML/CSS: For the front-end of the web app.

Future Enhancements

Add support for predicting classification labels (Fire/Not Fire).
Improve the web interface with more advanced visualization tools.
Include more machine learning models for comparison.

Acknowledgments

Dataset: Algerian Forest Fires Dataset - UCI Machine Learning Repository






