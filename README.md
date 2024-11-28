Vibration Analysis on Rotating Shaft


Overview

This project focuses on the analysis of vibration data collected from a rotating shaft. The primary goal is to understand the relationship between various input parameters such as voltage, RPM (Revolutions Per Minute), and vibration measurements, and to predict the force exerted on the shaft using a decision tree regression model.


Contents

Data Files: The project utilizes multiple CSV files containing vibration data, which are read into Pandas DataFrames for analysis.

Data Preprocessing: The code includes steps to clean and preprocess the data, including converting relevant columns to numeric types and handling missing values.

Feature Selection: The features selected for modeling include:

V_in: Input voltage

Measured_RPM: RPM of the shaft

Vibration_1, Vibration_2, Vibration_3: Different vibration measurements

Target Variable: The target variable for prediction is force, which is calculated based on the mass of the rotating shaft and its radius.

Modeling: A DecisionTreeRegressor from the sklearn library is used to fit the model on the preprocessed data.


Installation
To run this project, ensure you have the following Python packages installed:

pip install numpy pandas scikit-learn


Usage

Load the Data: The data is loaded from CSV files into Pandas DataFrames.

Preprocess the Data: Missing values are imputed, and columns are converted to numeric types.

Feature and Target Variables: Define the feature matrix X and target vector y.

Model Training: The decision tree regression model is trained on the processed data.

Prediction: Predictions can be made using the trained model on new data.

Example

An example of how to calculate the force exerted on the shaft is included in the code. The mass of the shaft and its radius are defined, and the force is computed using the formula:

k = mass * radius


Results

The model's performance can be evaluated using metrics such as R-squared score, which quantifies how well the model predictions match the actual data.


Conclusion

This project provides insights into the vibration characteristics of rotating shafts and demonstrates the application of machine learning techniques to predict mechanical forces based on sensor data. Further improvements could include exploring different regression models, hyperparameter tuning, and validating the model with additional datasets.
