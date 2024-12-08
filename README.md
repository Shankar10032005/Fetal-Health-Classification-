# Fetal Health Classification Using Machine Learning

## Project Overview:
This project focuses on developing a machine learning model to classify fetal health outcomes based on Cardiotocogram (CTG) test data. CTGs are essential tools in prenatal care, monitoring fetal heart rate, uterine contractions, and fetal movements. By building an automated machine learning system, this project aims to improve the accuracy and efficiency of interpreting CTG data, assisting healthcare professionals in making timely decisions to reduce maternal and child mortality.

The system classifies fetal health into three categories:
- **Normal**
- **Suspect**
- **Pathological**

The goal is to enhance early detection of fetal distress, thus contributing to better health outcomes in low-resource settings.

## Problem Statement:
Accurate interpretation of CTG results is crucial but often subjective and reliant on expert analysis. The aim of this project is to develop a machine learning-based approach to automatically classify CTG outcomes, thus enabling better and timely interventions to prevent fetal distress and reduce maternal mortality.

## Methodology:
The project follows a structured approach:
1. **Data Collection**: Using the Cardiotocogram (CTG) dataset, which contains 2126 records of features extracted from CTG exams.
2. **Preprocessing**:
   - **Handling Missing Data**: Identifying and handling missing values through imputation or removal.
   - **Outlier Detection**: Using box plots and the IQR method to detect and handle outliers.
   - **Data Splitting**: Dividing the dataset into training and testing sets.
3. **Model Selection**: Various machine learning models, including Logistic Regression, Decision Trees, Random Forest, and Support Vector Machine, are applied to predict fetal health status.
4. **Evaluation**: The models are evaluated based on accuracy, precision, recall, and F1 score.

## Data Set:
The dataset used in this project contains 2126 records, with features extracted from CTG exams. These records are classified by obstetricians into the following categories:
- **Normal**
- **Suspect**
- **Pathological**

## Data Analysis:
Key data analysis techniques used:
- **Strip Plot**: Visualizing categorical data distribution.
- **Correlation Matrix**: Exploring relationships between different features.
- **Boxen Plot**: Visualizing data distributions with enhanced details.
- **LMPlot**: Visualizing relationships with linear regression fit.

## Machine Learning Models:
The following models are implemented and compared:
- **Logistic Regression**: For binary classification, predicting fetal health outcomes.
- **Decision Tree Classifier**: For providing interpretable decision rules based on CTG features.
- **Random Forest Classifier**: An ensemble method combining multiple decision trees to improve classification accuracy.
- **Support Vector Machine (SVM)**: Effective for classifying fetal health into different categories.

## Evaluation Metrics:
The models are evaluated using the following metrics:
- **Accuracy**: Proportion of correct predictions.
- **Precision**: Correct positive predictions.
- **Recall**: Ability to identify all positive instances.
- **F1 Score**: Harmonic mean of precision and recall.

## Findings:
- The **Random Forest model** outperformed other models, achieving high accuracy, precision, and recall, both on the training and testing datasets.
- A confusion matrix analysis revealed that the Random Forest model classified fetal health categories effectively with minimal misclassifications.

## Flask API Implementation:
- A Flask API is set up to serve the trained Random Forest model. The API accepts input features from CTG data, predicts fetal health status (Normal, Suspect, Pathological), and returns the prediction to the user.
- The API provides a scalable solution for integrating fetal health monitoring into clinical settings, offering a user-friendly way to make predictions based on new CTG data.

## Conclusion:
The project successfully demonstrates how machine learning can automate the interpretation of CTG data, providing more accurate and timely fetal health assessments. The Random Forest model was particularly effective, and the implementation of the Flask API allows easy deployment in healthcare environments.


