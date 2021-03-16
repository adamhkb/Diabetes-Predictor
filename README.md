# Diabetes Predictor

Diabetes is one of the leading causes of death in the world, according to the World Health Organisation. Diabetes is a metabolic disease categorised by high levels of blood sugar, which can cause damage to the heart, kidneys, pancreas and many more organs. Diabetes occurs when the body is unable to use the insulin it produces, given that the pancreas does not produce enough insulin. According to WHO, an estimated of 1.6 million deaths were directly caused by diabetes in 2016.

This notebook looks into using Python-based Machine Learning and Data Science libraries in an attempt to build a Machine Learning model capable of predicting whether or not someone has diabetes based on their medical attributes.

## Problem Definition

A prediction of diabetes at an early stage of the disease can lead to an improved treatment that doctors can use, this can be achieved with the help of machine learning and data analytics. The aim of this assessment is to build a machine learning model to predict whether or not a patient has diabetes based on their medical attributes. Since the diabetes predictor has only two output, it is considered as a binary classification, given that it involves deciding whether a sample is part of one class or another.

## Data

The data that I have used came from Pima Indian Diabetes Database from UCI Machine Learning Repository. The dataset was downloaded in a formatted way from Kaggle. The downloaded dataset contains 9 attributes. Attributes are the variables that will be used to predict the target variable. Attributes and features are also referred to as independent variables and a target variable can be referred to as a dependent variable. In this case, the independent variables are a patient’s different medical attributes and the dependent variable is whether or not they have heart disease.

The dataset is available here: https://www.kaggle.com/uciml/pima-indians-diabetes-database 

## Features

Features are different parts of the data. The following are the features that will be used to predict our target variable (diabetes or no diabetes):
-    Pregnancies
-    Glucose
-    Blood Pressure
-    Skin Thickness
-    Insulin
-    BMI
-    Diabetes Pedigree function
-    Age
-    Outcome (diabetes or no diabetes)

## Tools

At the start of any project, it is crucial to prepare the tools for the project:
-    pandas for data analysis.
-    NumPy for numerical operations.
-    Matplotlib/seaborn for plotting or data visualisation.
-    Scikit-Learn for machine learning modelling and evaluation.

## Procedure 

### Data Exploration (Exploratory Data Analysis)

Once the dataset has been imported, the next step is to explore. The goal here is to find out more about the data and become a subject matter expert on the dataset of the project. A correlation matrix is a good method to analyse the data, given that it displays the correlation between independent variables.

### Modelling

Once the data has been explored, machine learning will be used to predict the target variable based on the 8 independent variables. One of the most important concepts in machine learning is splitting the data into a training set and a test set, the sets must remain separate. Once the data is prepared, we can start to fit models. Since this is a classification problem, the following models can be used and their results can be compared with each other:
-    Logistic Regression
-    K-Nearest Neighbours
-    Random Forest

Once the models have ran the testing and training sets required to get the accuracy score, It is importance to do the following:
-    Hyperparameter tuning: Each model that is used can be tuned to dictate how they perform. This could lead to better or worse model performance.
-    Feature importance: It is important to acknowledge which independent variable is crucial to achieve the target variable.
-    Confusion matrix: Compares predicted and true values in a tabular way.
-    Cross-validation: Splits the dataset into multiple parts and train and test your model on each part and evaluates performance as an average.
-    Precision: Indicates the proportion of positives identifications which were correct.
-    Recall: Indicates the proportion of actual positives which were correctly classified.
-    F1 Score: Combines precision and recall into one metric.
-    Classification Report: Built-in function which returns some of the main classification metrics.
-    ROC Curve: A plot of true positives rate versus false positive rate.
