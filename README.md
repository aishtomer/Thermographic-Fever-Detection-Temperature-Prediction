# Thermographic Fever Detection & Temperature Prediction

The project focuses on using sensor-collected data to predict oral temperature and detect fever using the **Infrared Thermography Temperature Dataset** from the UCI Machine Learning Repository.

## Problem Description

In this coursework, the goal is to predict:
1. Oral temperature measured in **fast mode** (`aveOralF`) – a regression task.
2. Oral temperature measured in **monitor mode** (`aveOralM`) – a regression task.
3. Whether a person has fever based on `aveOralF` and `aveOralM` (fever defined as oral temperature ≥ 37.5°C) – a classification task.

The dataset includes environmental variables such as ambient temperature and humidity, as well as thermal image readings from various body locations, which serve as input features for prediction.

## Project Objectives
- Build models to predict `aveOralF` and `aveOralM` using **regression** methods.
- Classify fever based on `aveOralF` and `aveOralM` using **classification** methods.
- Evaluate the models' performances using various metrics including RMSE, MAE (for regression) and precision, recall, F1-score, ROC AUC (for classification).
- Optimise the models using techniques such as hyperparameter tuning and feature importance analysis.
- Interpret the model results to provide insights into the most predictive variables.

## Methodology
### 1. Data Exploration and Preparation
- Initial exploration of data for missing values, outliers, and data distribution.
- Feature scaling and encoding for categorical variables.
- Splitting the dataset into training and testing sets.

### 2. Model Training
- Trained various regression models including:
  - **Linear Regression**
  - **Polynomial Regression**
  - **Neural Networks**
- For the classification tasks, trained several models:
  - **Logistic Regression**
  - **Random Forest Classifier**

### 3. Model Evaluation
- Regression metrics: RMSE, MAE, R² score.
- Classification metrics: accuracy, precision, recall, F1-score, ROC AUC, and confusion matrix.
- Precision/Recall trade-offs and AUC-PR used to choose optimal thresholds for fever classification.

## Results
- The performance of the regression and classification models are compared and evaluated.
- Feature importance analysis is conducted to understand the variables most impactful in predicting oral temperature and detecting fever.

## Technologies Used
- Python 3.9+
- Libraries: 
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

## Usage
1. Open the Jupyter notebook `Infrared_Thermography_Temperature_Prediction.ipynb` to view and run the analysis.
2. You can also explore the dataset by downloading it from the [UCI Repository](https://archive.ics.uci.edu/dataset/925/infrared+thermography+temperature+dataset).
