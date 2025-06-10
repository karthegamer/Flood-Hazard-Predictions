Flood Hazard Prediction Model
This project predicts soil flood hazard levels using a decision tree classifier trained on soil data from Washington State. The model processes and cleans the data, engineers features, trains a classifier, evaluates its performance, and outputs predictions for mapping.

Features:
  Loads and preprocesses soil data from CSV
  Feature engineering for soil properties and parent material
  Trains a decision tree classifier to predict flood hazard (SLIGHT, SEVERE, MODERATE)
  Evaluates model accuracy and visualizes confusion matrix and feature importances
  Outputs predictions to ai_flood_predictions.csv for mapping or other uses

Requirements:
  Python 3.x
  pandas
  numpy
  scikit-learn
  matplotlib
  alive-progress
  joblib
  
Install dependencies with:
  pip install pandas numpy scikit-learn matplotlib alive-progress joblib

Usage
  Place your soil data CSV as WA_Soils.csv in the same directory
  Run the script
  The script will:
    Load and preprocess the data
    Train and evaluate the model
    Output predictions to ai_flood_predictions.csv
    Show confusion matrix and feature importance plots
Output
  ai_flood_predictions.csv: Contains predicted flood hazard levels for each soil entry, mapped by OBJECTID.
Notes
  The script expects specific columns in the input CSV: OBJECTID, SOIL_PRNT_MAT, SOIL_PRECIP, SOIL_FLOOD_HAZARD, SOIL_DPT, SOIL_WATER_CAPY, SOIL_DRAIN_RATE.
  The model uses engineered features based on soil parent material and other properties.
