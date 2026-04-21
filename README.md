# Travel Analytics: Classification and Recommendation System

## Project Overview

This project is a machine learning-based travel analytics system designed to perform:
- User classification (gender prediction)
- Hotel recommendation based on user behavior
- Exploratory data analysis and insights generation

The objective is to enhance personalization in travel platforms using machine learning techniques.

---

## Problem Statement

The goal of this project is to:
- Predict user attributes such as gender using demographic data
- Build a recommendation system to suggest hotels based on user spending behavior
- Improve personalization and decision-making in travel services

---

## Dataset Description

### Users Dataset
- Columns: code, company, name, gender, age
- Used for classification tasks

### Hotels Dataset
- Columns: travelCode, userCode, name, place, days, price, total, date
- Used for building recommendation system

### Flights Dataset (if applicable)
- Used for exploratory analysis and feature insights

---

## Machine Learning Models

### 1. Classification Model
- Algorithm: Random Forest Classifier
- Target Variable: Gender
- Feature: Age

#### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

### 2. Recommendation System
- Approach: Top-N recommendation based on user spending behavior
- Method: Aggregation and ranking of hotels based on total spending per user

#### Evaluation Method:
- Top-N recommendation frequency analysis
- Popularity distribution of recommended hotels

---

## Project Workflow

1. Data loading
2. Data preprocessing and cleaning
3. Feature engineering
4. Model building
5. Model evaluation
6. Recommendation system development
7. Model saving using pickle/joblib
8. Prediction on unseen data

---

## Model Performance

The classification model using Random Forest provides:
- Good predictive accuracy
- Balanced precision and recall
- Stable performance on test data

The recommendation system effectively identifies popular hotels based on user behavior patterns.

---

## Model Saving

The trained model is saved using:
- Pickle (.pkl)
- Joblib (.joblib)

These files are used for deployment and future predictions.

---

## How to Run the Project

### Step 1: Clone the repository
```bash
git clone https://github.com/your-username/travel-analytics-project.git


## Step 2: Install dependencies

pip install -r requirements.txt

## Step 3: Run the notebook

Open Jupyter Notebook or Google Colab and execute:

Data preprocessing
Model training
Evaluation

## Step 4: Run Streamlit application (if available)
streamlit run app/app.py

Requirements
pandas
numpy
matplotlib
seaborn
scikit-learn
streamlit
joblib

Business Impact

Enables personalized travel recommendations
Improves marketing targeting efficiency
Enhances user engagement
Supports data-driven business decisions

Future Improvements

Deployment using Flask or FastAPI
Containerization using Docker
CI/CD pipeline integration
Experiment tracking using MLflow
Improved recommendation system using collaborative filtering

Conclusion

This project demonstrates an end-to-end machine learning pipeline for travel analytics, including classification and recommendation systems. It provides meaningful insights that can be used to improve user experience and business performance in travel platforms.
