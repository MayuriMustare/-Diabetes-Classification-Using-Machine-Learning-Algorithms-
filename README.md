# Diabetes Classification Using Machine Learning
## Project Description

This project is a Diabetes Classification System built using Machine Learning and Flask.
It predicts whether a person is diabetic or not based on medical input data.

A Random Forest Classifier is trained on a diabetes dataset and deployed through a Flask REST API to provide predictions.

## Technologies Used
### 1.Backend

   Python

   Flask

   Flask-CORS

   NumPy

   Pandas

   Scikit-learn
  
   Pickle

### 2.Frontend

   HTML

   CSS

## Dataset Used

Healthcare-Diabetes.csv

Diabetes_prediction.csv

The dataset contains medical attributes and an Outcome column indicating diabetes presence.

## Machine Learning Workflow

1. Load the dataset

2. Separate features and target variable (Outcome)

3. Scale features using StandardScaler

4. Select top 5 features using SelectKBest (ANOVA)

5. Apply PCA to reduce features to 3 components

6. Train Random Forest Classifier

7. Evaluate model using:

   a. Cross-validation

   b. Accuracy score

   c. Classification report

8. Save trained model using pickle

## Input Features

   Pregnancies

   Glucose

   Blood Pressure

   Skin Thickness

   Insulin

   BMI

   Diabetes Pedigree Function

   Age

For male users, the pregnancies value is automatically set to 0.

## Project Structure

Diabetes-Classification/
├── server.py
├── Healthcare-Diabetes.csv
├── Diabetes_prediction.csv
├── index.html
├── index.css
├── diabetes_rf_model.pkl
└── README.md











