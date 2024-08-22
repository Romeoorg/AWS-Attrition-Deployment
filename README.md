# Attrition Project Documentation

## Table of Contents
- [Abstract](#abstract)
- [Dataset Overview](#dataset-overview)
- [Exploratory Data Analysis (EDA) in Power BI](#exploratory-data-analysis-eda-in-power-bi)
- [Model Deployment Process Using Amazon SageMaker](#model-deployment-process-using-amazon-sagemaker)
- [Pre-requisites](#pre-requisites)
- [About the Dataset](#about-the-dataset)
- [Conclusion](#conclusion)

## Abstract
This document outlines the steps to train a logistic regression model using Amazon Sage Maker. It covers importing libraries, setting up the Sage Maker session, configuring the estimator, and managing input data. The guide provides clear instructions for setting hyperparameters and starting the training job, offering a concise roadmap for leveraging Sage Maker’s capabilities in machine learning.

## Dataset Overview
- **Dataset:** Synthetic Employee Attrition Dataset
- **Purpose:** Analyze and predict employee turnover.
- **Size:** 74,498 samples with detailed employee information.
- **Key Feature:** Attrition (0 = stayed, 1 = left).

## Exploratory Data Analysis (EDA) in Power BI
- **Distribution of Attrition:** Visual representation of the proportion of employees who left versus those who stayed.
- **Attrition by Job Role:** Analysis of attrition rates across different job roles.
- **Attrition by Job Satisfaction:** Examination of how job satisfaction impacts employee attrition.
- **Attrition by Work-Life Balance:** Analysis of the relationship between work-life balance and attrition.
- **Attrition by Marital Status:** Insights into how marital status correlates with attrition.
- **Pair Plot:** Visualizes relationships between selected features.

## Model Deployment Process Using Amazon SageMaker
1. **Create Notebook Instance:** Set up a development environment.
2. **Import Libraries:** Essential packages like pandas, boto3, and SageMaker.
3. **Load Data:** Import the dataset from the provided link.
4. **EDA Steps:**
   - View the first few rows.
   - Check for missing values.
   - Analyze key columns, especially Attrition.
5. **Data Preparation:**
   - Encode categorical data.
   - Filter and split data into training and testing sets.
6. **S3 Integration:** Upload data to S3 bucket using boto3.
7. **Model Training:**
   - Configure SageMaker Estimator with hyperparameters.
   - Start the training job.
8. **Model Deployment:**
   - Deploy the trained model on SageMaker.
   - Verify the deployment using test data.
9. **Lambda Function for Prediction:**
   - Create and configure a Lambda function to consume the model.
   - Use IAM roles for access management.
10. **Testing:**
   - Predictions: 0 = Employee stays, 1 = Employee leaves.

## Pre-requisites
Ensure that all necessary tools and libraries are installed, including access to AWS services like Sage Maker, S3, and Lambda.

## About the Dataset
The Synthetic Employee Attrition Dataset is designed for analyzing and predicting employee turnover. It includes 74,498 samples with detailed employee information such as demographics, job roles, and personal circumstances.

## Conclusion
In this project, we successfully developed a logistic regression model to predict employee attrition using the Synthetic Employee Attrition Dataset. The process involved multiple steps, from data preparation and exploratory data analysis to model training and deployment using Amazon SageMaker. This demonstrates the end-to-end process of building, training, and deploying a machine learning model in a cloud environment. The deployed model can now be used for HR analytics to predict employee turnover, providing valuable insights for decision-making. By leveraging Amazon SageMaker, the process was efficient and scalable, showcasing the power of cloud-based machine learning.

## References

- [Link to Dataset](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset?select=train.csv)
- Any other relevant links or references

## Contact

For any questions or contributions, feel free to contact me at [romeo.sebola@gmail.com](mailto:romeo.sebola@gmail.com).

