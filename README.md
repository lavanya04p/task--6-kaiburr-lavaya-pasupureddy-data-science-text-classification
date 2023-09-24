# Consumer_Complaint_Database_Text_Classification
This is Task-6 submission of Kaiburr Data Science Example

# Consumer Complaints Text Classification and Prediction (Multiclass)

## Task Description
This project involves performing text classification on consumer complaints using a publicly available dataset from the [Consumer Complaint Database](https://catalog.data.gov/dataset/consumer-complaint-database). The goal is to classify consumer complaints into predefined categories, such as credit reporting, debt collection, mortgage, and more.

## Table of Contents
- [Introduction](#introduction)
- [Data and Resources](#data-and-resources)
- [Data Preprocessing](#data-preprocessing)
- [Text Preprocessing](#text-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Multi-Classification Models](#multi-classification-models)
- [Model Comparison](#model-comparison)
- [Model Evaluation](#model-evaluation)
- [Predictions](#predictions)

## Introduction
Consumer complaints received about financial products and services are a valuable source of information. By classifying these complaints into specific categories, we can gain insights into the most common issues customers face and improve financial products and services.

## Data and Resources
- The dataset used in this project is obtained from the [Consumer Complaint Database](https://catalog.data.gov/dataset/consumer-complaint-database).
- Libraries such as Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, and others are utilized for data analysis, preprocessing, modeling, and evaluation.

## Data Preprocessing
- The dataset contains over a million instances and 18 features.
- Unnecessary features are removed to focus on 'Product' and 'Consumer complaint narrative.'
- Missing values (NaN) are removed from the 'Consumer complaint narrative' column.
- Categories are renamed and reduced from 18 to 13 for better classification.

## Text Preprocessing
- Text data is transformed into numerical vectors using Term Frequency-Inverse Document Frequency (TF-IDF) weighting.
- TF-IDF reflects the importance of words within documents and across the corpus.
- Stop words and punctuation are removed, and n-grams (unigrams and bigrams) are considered.

## Feature Engineering
- Features are extracted from the 'Consumer complaint narrative' text data using TF-IDF.

## Multi-Classification Models
- Two models are used for multi-class classification: Linear Support Vector Machine (LinearSVM) and Multinomial Naive Bayes.
- The models are trained and evaluated using cross-validation.

## Model Comparison
- Model performance is compared based on mean accuracy.
- LinearSVC achieves the highest mean accuracy.

## Model Evaluation
- Classification metrics including precision, recall, and F1-score are calculated.
- A confusion matrix visualizes the performance of the LinearSVC model.

## Predictions
- The trained LinearSVC model is used to make predictions on new consumer complaints.
- Example complaints are provided, and the model correctly classifies them.

This project demonstrates how text classification can be applied to real-world consumer complaints data to categorize and predict the nature of complaints, helping organizations better address customer concerns and improve their products and services.
