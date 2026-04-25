# Travel Analytics: End-to-End ML and MLOps System

## Project Overview

This project is a complete machine learning and MLOps-based travel analytics system designed to perform:

- Gender classification of users  
- Flight price prediction (regression)  
- Hotel recommendation system  
- Deployment using Streamlit and Flask  
- Basic MLOps integration (MLflow, Docker, Airflow concepts)  

The goal is to enhance personalization and decision-making in travel platforms using data-driven techniques.

---

## Problem Statement

The objective of this project is to:

- Predict user attributes such as gender using demographic data  
- Predict flight prices using travel-related features  
- Recommend hotels based on user behavior and spending patterns  
- Build a scalable and deployable ML system with MLOps practices  

---

## Dataset Description

### Users Dataset
- Columns: code, company, name, gender, age  
- Used for classification tasks  

### Hotels Dataset
- Columns: travelCode, userCode, name, place, days, price, total, date  
- Used for recommendation system  

### Flights Dataset
- Columns: travelCode, userCode, from, to, price, distance, time, etc.  
- Used for regression (price prediction)  

---

## Machine Learning Models

### 1. Classification Model (Gender Prediction)

- Algorithm: Random Forest Classifier  
- Feature: Age  
- Target: Gender  

#### Evaluation Metrics:
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

### 2. Regression Model (Flight Price Prediction)

- Algorithm: Random Forest Regressor  
- Features: Distance, Time  
- Target: Flight Price  

#### Evaluation Metrics:
- RMSE (Root Mean Squared Error)  
- R² Score  

---

### 3. Recommendation System (Hotels)

- Approach: Top-N recommendation  
- Method: Aggregation of total spend per user per hotel  

#### Evaluation:
- Most frequently recommended hotels  
- User-level top recommendations  

---

## Project Workflow

1. Data loading  
2. Data cleaning and preprocessing  
3. Feature engineering  
4. Model building (classification, regression)  
5. Model evaluation  
6. Recommendation system development  
7. Model saving (joblib/pickle)  
8. Deployment using Streamlit  
9. API development using Flask  
10. MLOps integration  

---

## Model Performance

- Classification model shows stable performance with balanced precision and recall  
- Regression model provides reasonable prediction accuracy for flight prices  
- Recommendation system identifies popular hotels based on user behavior  

---

## Deployment

### Streamlit Application

- Interactive UI for prediction  
- User input (age)  
- Real-time prediction output  

Run using:

```bash
streamlit run app.py
