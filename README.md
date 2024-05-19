# Taxi Trip Duration Prediction

## Overview
This project demonstrates a pipeline for predicting the duration of NYC taxi trips using a linear regression model. The data is processed, features are extracted and encoded, and the model's performance is evaluated using Root Mean Squared Error (RMSE).

## Requirements
- Python 3.6+
- Pandas
- PyArrow
- Scikit-learn

## Data
- NYC Yellow Taxi trip records in Parquet format
- Each record includes pickup and drop-off locations, and timestamps

## Usage

### Read Data:
- Convert pickup and drop-off times to datetime
- Calculate trip duration in minutes
- Retain trips with durations between 1 and 60 minutes

### Load Training and Validation Data: 
- Read the January dataset for training
- Read the February dataset for validation

### Feature Encoding:
- Convert categorical location IDs to string
- Encode using DictVectorizer

### Model Training:
- Train a linear regression model on the training data

### Evaluation:
- Calculate and print the RMSE for both training and validation datasets

## Acknowledgments
- DataTalksClub
