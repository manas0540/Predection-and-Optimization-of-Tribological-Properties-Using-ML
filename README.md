## Prediction and Optimization of Tribological Properties of 
copper- graphite-TiC composite under lubricating sliding 
condition by using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-green)
![Tribology](https://img.shields.io/badge/Domain-Tribology-orange)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-red)


Overview

This project predicts the Wear Rate (WR) and Coefficient of Friction (COF) of Copper–Graphite–Titanium Carbide (Cu-Gr-TiC) composites under lubricated sliding conditions using Machine Learning techniques.

The study combines tribological experimental data with machine learning models to reduce the need for expensive and time-consuming physical testing while enabling rapid material performance prediction.

Problem Statement

Traditional tribological experiments require significant time, resources, and laboratory effort.

The objective of this project is to develop data-driven predictive models capable of estimating:

Wear Rate (WR)
Coefficient of Friction (COF)

using process and material parameters.

Dataset Features
Input Features
Feature	Description
Load	Applied Load (N)
Distance	Sliding Distance (m)
Composition	TiC Reinforcement Content (wt%)
Target Variables
Target	Description
Wear Rate	Material wear during sliding
COF	Coefficient of Friction
Methodology
Data Collection
Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Correlation Analysis
Train-Test Split
Model Training
Model Evaluation
Prediction & Optimization
Machine Learning Models Used
Artificial Neural Network (ANN)
Hidden Layers: 64-32-16
Activation: ReLU
Optimizer: Adam
Random Forest Regression
Ensemble-based model
Robust against noise
Support Vector Regression (SVR)
RBF Kernel
Strong performance on small datasets
K-Nearest Neighbors (KNN)
Distance-based regression
Simple and interpretable model
Exploratory Data Analysis

Key observations:

Load showed a strong positive correlation with Wear Rate.
Load significantly influenced COF.
Increasing TiC content reduced Wear Rate.
TiC reinforcement improved tribological performance.
Evaluation Metrics

The following metrics were used:

MAE
RMSE
R² Score
MAPE

Results

Wear Rate Prediction
Model	R² Score
ANN	0.6497
Random Forest	0.7959
KNN	0.8106
SVR	0.8887

Best Model: SVR

COF Prediction
Model	R² Score
ANN	0.9619
Random Forest	0.7888
SVR	0.8387
KNN	0.7177

Best Model: ANN

Key Findings
SVR achieved the highest accuracy for Wear Rate prediction.
ANN achieved the highest accuracy for COF prediction.
Machine Learning can effectively replace a large number of experimental trials.
Higher TiC reinforcement improves wear resistance under lubricated conditions.
Technologies Used
Python
Pandas
NumPy
Matplotlib
Scikit-Learn
Jupyter Notebook


References
Ankit et al. (2023) – Prediction of tribological performance of Cu-Gr-TiC composites.
Huifeng Ning et al. (2024) – Machine Learning based tribological property prediction.



