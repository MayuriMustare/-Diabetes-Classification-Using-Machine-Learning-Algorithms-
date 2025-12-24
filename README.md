Diabetes Classification Using Machine Learning
Project Description

This project is a Diabetes Classification System developed using Machine Learning and Flask.
It predicts whether a person is diabetic or not based on medical attributes provided by the user.

The backend is implemented using Flask, where a Random Forest Classifier is trained on a diabetes dataset. The trained model is then used to serve predictions through REST API endpoints.

Technologies Used
Backend

Python

Flask

Flask-CORS

NumPy

Pandas

Scikit-learn

Pickle

Frontend

HTML

CSS (Tailwind-based styling)

Dataset Used

Healthcare-Diabetes.csv

Diabetes_prediction.csv

The dataset contains medical attributes such as glucose level, blood pressure, BMI, age, insulin level, etc., along with an Outcome column indicating diabetes presence.

Machine Learning Workflow

Load the diabetes dataset

Split features and target variable (Outcome)

Scale features using StandardScaler

Select top 5 features using SelectKBest (ANOVA)

Reduce features using PCA (3 components)

Train Random Forest Classifier

Evaluate model using:

Cross-validation

Accuracy score

Classification report

Save trained model using pickle

Input Features

The model uses the following input parameters:

Pregnancies

Glucose

Blood Pressure

Skin Thickness

Insulin

BMI

Diabetes Pedigree Function

Age

For male users, the pregnancies value is automatically set to 0.
