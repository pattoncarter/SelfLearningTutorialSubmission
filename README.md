This project examines Flaredown's Chronic illness: symptoms, treatments and triggers dataset of Kaggle, https://www.kaggle.com/datasets/flaredown/flaredown-autoimmune-symptom-tracker?resource=download

Patient Condition Prediction from Self-Reported Symptoms

This project explores the use of machine learning on self-reported patient symptom data to predict chronic condition labels. Patients track daily symptoms and conditions through the Flaredown app, and we leverage this data to build a predictive model.

Overview

Data Ingestion and Cleaning:
The raw data is preprocessed to remove extraneous punctuation and formatting (e.g., newline and quote characters). We pivot the data into a "patient fingerprint" where each row represents a patient and each column is a symptom with the corresponding average severity.
Feature Engineering:
We clean and standardize the symptom data to ensure that the model sees a consistent, well-scaled input. Additional preprocessing includes stripping unwanted punctuation and characters.
Model Training:
Using 80% of the data for training, we built a Feedforward Multilayer Perceptron (MLP) that learns to predict a patient’s primary condition (taken as the ground truth) from their symptom fingerprint. The remaining 20% is held out for testing, and the model's performance is evaluated on this set.
Interactive Prediction:
An interactive section allows users to input a symptom and its severity to see the condition that the model associates with that symptom profile. This interactive element makes the model accessible and engaging, even to those without a technical background.

Getting Started

Prerequisites
Python 3.7+
Required libraries: pandas, numpy, matplotlib, scikit-learn
