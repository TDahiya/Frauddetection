# Fraud Detection Model

## Introduction
This project implements a fraud detection model using a Random Forest classifier. The model aims to identify fraudulent transactions based on various features in the dataset.

## Description
The `Model.ipynb` Jupyter Notebook contains the implementation of the fraud detection model. Below is an overview of the key sections of the code:

### Importing Libraries
- Libraries such as Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, and SciPy are imported for data manipulation, visualization, and model building.

### Data Loading and Cleaning
- The dataset `Fraud.csv` is loaded into a Pandas DataFrame.
- Irrelevant columns (`nameOrig`, `nameDest`) are dropped.
- Missing values are handled by dropping rows with missing values.

### Data Preprocessing
- Categorical features are one-hot encoded using Pandas `get_dummies` function.

### Train-Test Split
- The data is split into training and testing sets using Scikit-learn's `train_test_split` function.

### Feature Scaling
- Features are scaled using Scikit-learn's `StandardScaler`.

### Model Training
- A Random Forest classifier with 100 estimators is trained on the scaled training data.

### Model Evaluation
- The model is evaluated on the test set using metrics like confusion matrix and classification report.

### Feature Importance Analysis
- Feature importances are computed and visualized using a bar plot to understand the significance of each feature in the model.

### Model Prediction
- The trained model is used to predict fraud on the full dataset, and a bar plot compares actual fraud counts with predicted fraud counts.

## Results
- The model demonstrates satisfactory performance in detecting fraudulent transactions.
- Feature importance analysis reveals key factors contributing to fraud detection.


