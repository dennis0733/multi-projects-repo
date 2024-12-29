# Algerian Forest Fires FWI Prediction

## Overview
This project implements a machine learning solution to predict the Fire Weather Index (FWI) using environmental and meteorological data from two regions in Algeria. The system utilizes various regression techniques and is deployed as a web application using Flask.

## Dataset Description
The project uses the [Algerian Forest Fires Dataset](https://archive.ics.uci.edu/dataset/547/algerian+forest+fires+dataset) from the UCI Machine Learning Repository, which includes:
- 244 instances (equally split between Bejaia and Sidi Bel-abbes regions)
- Collection period: June 2012 to September 2012
- 11 environmental and weather-related features
- Fire Weather Index (FWI) as the target variable
- Class distribution: 138 fire instances, 106 non-fire instances

### Features
- Temperature
- Relative Humidity
- Wind Speed
- Rainfall
- And other environmental parameters

## Project Structure
```
algerian_forest_fires/
├── application.py              # Flask web application
├── requirements.txt            # Project dependencies
├── data/
│   ├── Algerian_forest_fires_dataset_UPDATE.csv
│   └── cleaned_dataset.csv
├── models/
│   ├── ridge.pkl              # Trained model
│   └── scaler.pkl             # Data preprocessor
├── notebooks/
│   ├── EDA_fires.ipynb        # Data analysis
│   └── model_training.ipynb   # Model development
└── templates/
    ├── index.html             # Input form
    └── home.html              # Results page
```

## Machine Learning Models
The project evaluates multiple regression models:
- Linear Regression
- Ridge Regression (selected as best performing)
- Lasso Regression
- ElasticNet Regression

## Installation

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/algerian-forest-fire-prediction.git
cd algerian-forest-fire-prediction
```

2. **Create Virtual Environment**
```bash
# Create environment
python -m venv venv

# Activate environment
# For Windows:
venv\Scripts\activate
# For macOS/Linux:
source venv/bin/activate
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the Application**
```bash
python application.py
```

Access the web interface at `http://127.0.0.1:5000/`

## Usage Guide

1. Navigate to the web application
2. Enter the required environmental parameters:
   - Temperature
   - Relative Humidity
   - Wind Speed
   - Rainfall
   - Additional parameters as prompted
3. Submit the form to receive the predicted Fire Weather Index

## Technologies Used

- **Backend Development**
  - Python 3.x
  - Flask
  - Scikit-learn

- **Data Processing**
  - Pandas
  - NumPy
  - Scikit-learn preprocessing tools

- **Frontend**
  - HTML
  - CSS

## Future Development Plans

1. **Enhanced Prediction Capabilities**
   - Implementation of fire/no-fire classification
   - Integration of additional machine learning models
   - Model performance optimization

2. **User Interface Improvements**
   - Advanced data visualization features
   - Interactive result analysis tools
   - Batch prediction capabilities

3. **System Enhancements**
   - API endpoint development
   - Enhanced error handling
   - Comprehensive logging system
   - 
## Acknowledgments

- UCI Machine Learning Repository for the Algerian Forest Fires Dataset
- The scientific community for research in forest fire prediction
- Contributors and maintainers of the open-source libraries used in this project
