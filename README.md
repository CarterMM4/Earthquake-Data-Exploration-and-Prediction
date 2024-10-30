# Earthquake-Data-Exploration-and-Prediction
Analyzes global earthquake data to explore magnitude distribution, temporal trends, and geographic patterns. Includes data cleaning, feature engineering, and a predictive model using Random Forest Regressor. Visualizes key insights and evaluates model performance with Mean Squared Error and R² score.

Earthquake Data Analysis and Magnitude Prediction:

This project explores a global earthquake dataset, performing in-depth analysis, visualizations, and predictive modeling. The goal is to uncover patterns in earthquake occurrences and build a model to predict earthquake magnitudes based on geographical and temporal features.

Project Overview:

Data Preprocessing: Cleans and prepares the data by handling missing values, converting date formats, and encoding categorical features.
Exploratory Data Analysis (EDA): Visualizes the distribution of earthquake magnitudes, trends over time, and geographical locations to reveal patterns.
Feature Engineering: Generates additional features, such as month and day, and scales numerical features to optimize model performance.
Predictive Modeling: Applies a Random Forest Regressor to predict earthquake magnitudes. Dimensionality reduction via PCA enhances the model by simplifying input features.
Model Evaluation: Assesses model performance using Mean Squared Error (MSE) and R² score, with a feature importance plot to highlight influential factors.

Requirements:

Python 3.x
Libraries: pandas, seaborn, matplotlib, scikit-learn, kaggle

How to Run:

Kaggle Setup: Upload kaggle.json for API access.
Data Download: Automatically downloads and unzips the dataset using the Kaggle API.
Run Code: Each step is detailed in the notebook, with plots and evaluation metrics provided.
This project demonstrates practical data analysis, feature engineering, and predictive modeling skills, useful for anyone interested in data science or seismology.
