# Smart_Irrigation_AICTE_SHELL_Proj1
This is an AICTE Internship Project

Project Overview
Traditional irrigation systems often rely on manual operation or simple timers, leading to water wastage or suboptimal irrigation. This project automates and optimizes sprinkler activation in agricultural fields using real-time data from 19 sensors and a machine learning classification model. Users enter current sensor readings and the app predicts which sprinklers (parcels) should be ON or OFF, conserving water and boosting crop health.

Features
Real-time input of up to 19 sensor readings via an interactive Streamlit UI.

ML-based prediction for each sprinkler's ON/OFF status.

Automatic, data-driven irrigation decisions for sustainable water management.

Modular code, easy retraining and model updates.

Ready for extension to larger fields, additional sensor types, or new algorithms.

Problem Statement
Manual or rule-based irrigation wastes precious water resources and may cause crop stress due to under- or over-watering. We need a smart solution that:

Monitors key environmental and crop parameters in real-time.

Automates irrigation decisions via a machine learning model for 19 sensor zones.

Reduces water/energy usage, increasing efficiency and sustainability.

Solution Approach
Data Collection: Gather sensor data (soil moisture, humidity, temperature, etc.) labeled with required sprinkler actions.

Preprocessing: Clean, handle outliers, normalize sensor readings.

EDA & Visualization: Analyze trends, sensor correlations, and predictive features.

Model Building: Train a classification model (e.g., Random Forest) to predict ON/OFF for each sprinkler.

Deployment: Bundle the trained model via joblib and integrate with a Streamlit web application.

User Interface: Easily enter sensor values and instantly get sprinkler activation suggestions.

Tools & Technologies
Language: Python 3.9+

Libraries:

numpy, pandas (data processing)

scikit-learn (ML algorithms)

matplotlib, seaborn (EDA/visualization)

joblib (model persistence)

streamlit (web app)

Development Environment: Jupyter Notebook, Streamlit Cloud/Local, VS Code

Version Control: Git, GitHub

Methodology
Data Collection: Simulated or real multi-sensor dataset, 19 sensors per observation, labeled with sprinkler status (ON/OFF).

Preprocessing: Missing value imputation, normalization ( scaling), label encoding.

Exploratory Data Analysis:

Sensor distribution plots

Correlation matrices

Investigation of water use and prediction logic

Modeling:

Train/test split

Model selection (RandomForest, DecisionTree, etc.)

Evaluation using accuracy, confusion matrix, and feature importance.

App Deployment:

Farm_Irrigation_System.pkl model saved with joblib.

Streamlit app gets 19 sensor values using sliders, performs prediction, displays ON/OFF per parcel.

How to run?

Clone the Repository

git clone https://github.com/yogi2022/Smart_Irrigation_AICTE_SHELL_Proj1.git
cd Smart_Irrigation_AICTE_SHELL_Proj1

Install Dependencies

pip install -r requirements.txt

Run Streamlit App

streamlit run app.py


Smart_Irrigation_AICTE_SHELL_Proj1/
├── app.py                  # Streamlit app code
├── Farm_Irrigation_System.pkl   # Saved ML model
├── Irrigation_1.ipynb      # Model building and analysis notebook
├── Irrigation_2.ipynb      # App logic and testing notebook
├── requirements.txt        # Python dependencies
└── README.md               # This file

Results:

Accurate ON/OFF predictions for all 19 parcels based on sensor data

Significant savings in water and improved crop response (see EDA/Results in notebooks)

User-friendly interface enables rapid adoption and real-world validation
