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

## Installation and Setup
### Step 1: Clone the Repository

git clone https://github.com/your-username/diabetes-classification.git
cd diabetes-classification

### Step 2: Create Virtual Environment (Optional)
python -m venv venv

Activate the environment:
Windows

venv\Scripts\activate

Linux / macOS

source venv/bin/activate

### Step 3: Install Required Libraries

pip install flask flask-cors numpy pandas scikit-learn

Running the Application
python server.py

The Flask server will run at:
http://127.0.0.1:5000/

# API Endpoints
## Predict Diabetes

Endpoint:
POST /predict

Request Format (JSON):
{
  "gender": "female",
  "pregnancies": 2,
  "glucose": 120,
  "bloodPressure": 70,
  "skinThickness": 20,
  "insulin": 85,
  "bmi": 28.5,
  "diabetesPedigreeFunction": 0.5,
  "age": 32
}

Response:

{
  "result": "No diabetes detected!",
  "selected_features": ["Glucose", "BMI", "Age", "Insulin", "BloodPressure"]
}
