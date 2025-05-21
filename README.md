# Houseing-Price-Predictor

## Description

This project focuses on predicting the median house value in California using the California Housing Dataset. The goal is to build and compare different regression models that can accurately estimate house prices based on various features of housing districts. The project involves data loading, cleaning, preprocessing, feature engineering, and training machine learning models.

### Data

The dataset used in this project is the California Housing Dataset. It is assumed that the dataset is available as a CSV file named `housing.csv` in the same directory as the notebook.

# Code Overview

- **Data Loading and Preprocessing:** The code loads the `housing.csv` file, handles missing values by dropping rows, and applies logarithmic transformation to some numerical features. Categorical features are one-hot encoded.
- **Feature Engineering:** New features like 'rooms_per_household' and 'bedrooms_per_room' are created.
- **Data Splitting:** The data is split into training and testing sets.
- **Model Training:**
    - A Linear Regression model is trained on the training data.
    - A Random Forest Regressor model is trained on the training data.
- **Scaling:** The numerical features are scaled using StandardScaler before training the Linear Regression model (although the scaling is applied to the original X_train/X_test, not used in the linear regression model training in the provided code).

## Future Enhancements

- Evaluate the models using appropriate regression metrics (e.g., R-squared, Mean Squared Error).
- Tune the hyperparameters of the models for better performance.
- Explore other regression models.
- Implement cross-validation for more robust model evaluation.
- Visualize the results and analyze feature importances.
