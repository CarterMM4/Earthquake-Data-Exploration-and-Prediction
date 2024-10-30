# Earthquake Analysis and Magnitude Prediction with Machine Learning
This project analyzes a global earthquake dataset to explore earthquake patterns, visualize key insights, and build a machine learning model to predict earthquake magnitudes. By leveraging data cleaning, exploratory analysis, feature engineering, and predictive modeling, this project provides insights into earthquake occurrences and highlights the factors that influence earthquake severity.

# Project Structure
1. Kaggle API Setup and Data Download:

Uses the Kaggle API to download and access the earthquake dataset from the US Geological Survey (USGS).
Requires a kaggle.json file with API credentials, which is securely configured within the environment.

2. Data Loading and Inspection:

The dataset is loaded into a Pandas DataFrame and initially inspected to understand column names, data types, and missing values.
Key columns such as IDs and source indicators are removed as they don’t contribute to the analysis or model.

3. Data Preprocessing:

Converts the Date column to a datetime format to enable time-based analysis.
Fills missing values: numerical columns are filled with the median, while categorical columns (e.g., Type) are filled with a placeholder, 'Unknown'.
These preprocessing steps ensure that the dataset is clean, consistent, and suitable for further analysis and modeling.

4. Exploratory Data Analysis (EDA):

Magnitude Distribution: Visualizes the frequency distribution of earthquake magnitudes with a histogram and density plot to reveal common magnitude levels.
Yearly Earthquake Frequency: Extracts the year from each earthquake's date to observe earthquake frequency trends over time, displayed as a count plot.
Geographic Distribution: Plots earthquake locations on a scatterplot with color-coding by magnitude, providing a spatial view of earthquake activity worldwide.

5. Feature Engineering:

Date-Based Features: Extracts Month and Day from the Date column to capture potential seasonal or monthly trends in earthquake occurrences.
Encoding Categorical Data: One-hot encodes the Type column to allow categorical features to be incorporated into the predictive model.
Scaling Numerical Features: Scales latitude, longitude, depth, month, and day using standard scaling to improve model performance by normalizing feature ranges.

6. Predictive Modeling:

Defines X (feature variables) and y (target variable, Magnitude) to prepare the data for machine learning.
PCA for Dimensionality Reduction: Applies Principal Component Analysis (PCA) to reduce the feature set to five principal components, simplifying the data while retaining key information.
Random Forest Regressor: Trains a Random Forest model to predict earthquake magnitudes based on location, depth, and time-based features. This model is evaluated using Mean Squared Error (MSE) and R² score, providing metrics for accuracy and variance explained.

7. Feature Importance Visualization:

Plots the importance of each feature based on the trained Random Forest model, highlighting the most influential variables for predicting earthquake magnitude.

# Requirements

Python Libraries:
  - pandas for data manipulation and cleaning
  - seaborn and matplotlib for data visualization
  - scikit-learn for machine learning and PCA
  - kaggle for dataset access

Additional Setup: Upload kaggle.json to access Kaggle datasets.

# How to Use
  1. Upload kaggle.json to authenticate with the Kaggle API.
  2. Run the cells sequentially to download the data, preprocess it, perform analysis, and train the prediction model.
  3. Review visualizations and model evaluation metrics to interpret findings.

# Project Insights
This project demonstrates practical skills in data cleaning, feature engineering, exploratory analysis, and machine learning. By analyzing earthquake characteristics and predicting magnitude, this project provides a framework for geospatial data analysis and a foundation for further research in earthquake forecasting.
