# Weather-Projection 
Wildfire Burned Area Prediction
This repository contains a Flask web application that predicts the burned area of forest fires using a Ridge regression model. The application uses environmental variables as input and displays the burned area in hectares.

#Table of Contents
Features
Demo
Project Structure
Installation
Usage
Model Training
License

#Features
User-friendly UI built with Bootstrap 5
Nine environmental input variables: Temperature, Relative Humidity, Wind Speed, Rain, FFMC, DMC, ISI, Classes, Region
Pretrained Ridge regression model with standardized inputs
Prediction results displayed in hectares

#Demo
Navigate to the home page and enter the environmental variables.
Click Predict to see the estimated burned area (in hectares).
View the result on a clean, responsive results page.

#Project Structure
text
project/
├── app.py                   # Flask application
├── models/
│   ├── ridge.pkl            # Pretrained Ridge regression model
│   └── scaler.pkl           # Standard scaler object
├── notebooks/
│   ├── forest.ipynb         # Data exploration & preprocessing
│   └── model.ipynb          # Model training & evaluation
├── static/
│   ├── css/
│   │   └── styles.css       # Custom styles
│   └── js/
│       └── scripts.js       # (Optional) custom scripts
├── templates/
│   ├── index.html           # Input form page
│   └── home.html            # Prediction result page
└── README.md                # Project documentation
Installation
Clone the repository

#bash
git clone https://github.com/your-username/fire-area-predictor.git
cd fire-area-predictor
Create and activate a virtual environment

bash
python3 -m venv venv
source venv/bin/activate
Install dependencies

bash
pip install -r requirements.txt
Download or place the ridge.pkl and scaler.pkl files in the models/ directory.

#Usage
Run the Flask app

bash
python app.py
Open your browser to http://127.0.0.1:5000/

Enter values for all input fields and submit to view the prediction.

#Model Training
All data exploration and model training steps are documented in the Jupyter notebooks:

notebooks/forest.ipynb:

Data loading, cleaning, and exploratory analysis (feature distributions, correlation heatmap).

notebooks/model.ipynb:

Standard scaling, Ridge regression training, hyperparameter tuning, and model evaluation (residual plots, metrics).


