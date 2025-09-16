Network Security Detection Project
Project Overview

This project implements a complete end-to-end machine learning pipeline for detecting network security threats using data-driven techniques. The system is designed in a modular and scalable way so that new data can be easily ingested, validated, transformed, and used for model training and evaluation.

The main objective of this project is to build an automated Network Threat Detection System using classification algorithms to classify network traffic or datasets into categories such as normal and phishing/malicious activity.

Project Features

Data Ingestion:

Fetch data from MongoDB collections.

Store raw and ingested data in organized artifact folders with timestamps.

Split data into training and testing sets for model development.

Data Validation:

Verify that incoming data meets the schema requirements.

Check for missing values, duplicate records, and correct number of columns.

Detect data drift between training and new incoming data.

Generate a DataValidationArtifact for further pipeline steps.

Data Transformation:

Preprocess the data and save the transformed training and testing arrays.

Store preprocessing objects (like encoders, scalers) for consistent transformation during inference.

Save transformed data in .npy format for efficient model training.

Model Training and Selection:

Train multiple classification models including:

Random Forest, Decision Tree, Gradient Boosting

Logistic Regression, AdaBoost

Perform hyperparameter tuning and select the best-performing model based on metrics.

Save the trained model along with preprocessing objects for production use.

Generate detailed classification metrics for both training and testing datasets.

Artifacts and Logging:

All intermediate outputs (raw data, feature store, transformed data, trained models, validation reports) are saved in artifacts folder with timestamped subdirectories.

Logging is implemented to track pipeline execution and debug errors.