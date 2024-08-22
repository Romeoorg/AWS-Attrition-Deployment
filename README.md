# AttritionAWSDeployment
Title
Attrition Project Documentation: A Comprehensive Guide to Training a Logistic Regression Model Using Amazon SageMaker

Introduction
This repository contains the documentation and code for training a logistic regression model to predict employee attrition using Amazon SageMaker. The guide provides a detailed walkthrough of the entire process, from data preparation and exploratory data analysis (EDA) in Power BI to model training, deployment, and prediction using AWS services.

Table of Contents
Abstract
Dataset Overview
Exploratory Data Analysis (EDA)
Model Deployment Process
Pre-requisites
Code Snippets
Conclusion
References
Abstract
This document outlines the steps to train a logistic regression model using Amazon SageMaker. It covers importing libraries, setting up the SageMaker session, configuring the estimator, and managing input data. The guide offers a concise roadmap for leveraging SageMaker's capabilities in machine learning.

Dataset Overview
Dataset: Synthetic Employee Attrition Dataset
Purpose: Analyze and predict employee turnover.
Size: 74,498 samples with detailed employee information.
Key Feature: Attrition (0 = stayed, 1 = left).
Exploratory Data Analysis (EDA)
The EDA was performed using Power BI to visualize various aspects of the dataset:

Distribution of Attrition: Shows the proportion of employees who left vs. those who stayed.
Attrition by Job Role: Analyzes attrition rates across different job roles.
Attrition by Job Satisfaction: Examines how job satisfaction impacts attrition.
Attrition by Work-Life Balance: Investigates the relationship between work-life balance and attrition.
Attrition by Marital Status: Correlates marital status with attrition.
Pair Plot: Visualizes relationships between selected features.
Model Deployment Process
Create Notebook Instance: Set up a development environment in SageMaker.
Import Libraries: Essential packages like pandas, boto3, and sagemaker.
Load Data: Import the dataset.
EDA Steps: Perform initial data exploration.
Data Preparation: Encode categorical data, split data into training and testing sets.
S3 Integration: Upload data to S3 bucket using boto3.
Model Training: Configure SageMaker Estimator and start the training job.
Model Deployment: Deploy the trained model on SageMaker.
Lambda Function for Prediction: Create and configure a Lambda function for predictions.
Testing: Run predictions using test data.
Pre-requisites
Ensure that all necessary tools and libraries are installed, including access to AWS services like SageMaker, S3, and Lambda.

Code Snippets
This section includes essential code snippets for tasks like:

Uploading a file to S3
Configuring SageMaker Estimator
Deploying the model
Creating Lambda functions for predictions
Conclusion
This project successfully developed and deployed a logistic regression model to predict employee attrition using the Synthetic Employee Attrition Dataset. The process showcases the end-to-end application of cloud-based machine learning with Amazon SageMaker, providing valuable insights for HR analytics.

References
Link to Dataset
Any other relevant links or references
Contact
For any questions or contributions, feel free to contact me at romeo.sebola@gmail.com.

