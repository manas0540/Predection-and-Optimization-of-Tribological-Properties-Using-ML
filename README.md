# Prediction and Optimization of Tribological Properties of Copper–Graphite–TiC Composite under Lubricating Sliding Condition using Machine Learning

## Overview

This project predicts the **Wear Rate (WR)** and **Coefficient of Friction (COF)** of **Copper–Graphite–Titanium Carbide (Cu–Gr–TiC) composites** under lubricated sliding conditions using Machine Learning techniques.

The study combines **tribological experimental data** with **machine learning models** to reduce the need for expensive and time-consuming physical testing while enabling rapid material performance prediction.

---

## Problem Statement

Traditional tribological experiments require significant time, resources, and laboratory effort.

The objective of this project is to develop **data-driven predictive models** capable of estimating:

- Wear Rate (WR)
- Coefficient of Friction (COF)

using process and material parameters.

---

## Dataset Features

### Input Features

| Feature | Description |
|----------|------------|
| Load | Applied Load (N) |
| Distance | Sliding Distance (m) |
| Composition | TiC Reinforcement Content (wt%) |

### Target Variables

| Target | Description |
|---------|------------|
| Wear Rate (WR) | Material wear during sliding |
| Coefficient of Friction (COF) | Frictional resistance between surfaces |

---

## Methodology

The workflow followed in this study is:

1. **Data Collection**
2. **Data Cleaning and Preprocessing**
3. **Exploratory Data Analysis (EDA)**
4. **Correlation Analysis**
5. **Train-Test Split**
6. **Model Training**
7. **Model Evaluation**
8. **Prediction and Optimization**

---

## Machine Learning Models Used

### 1. Artificial Neural Network (ANN)

- Hidden Layer Architecture: **64-32-16**
- Activation Function: **ReLU**
- Optimizer: **Adam**
- Suitable for capturing complex nonlinear relationships.

### 2. Random Forest Regression (RF)

- Ensemble-based regression model.
- Robust against noisy data.
- Reduces overfitting through multiple decision trees.

### 3. Support Vector Regression (SVR)

- Kernel: **RBF (Radial Basis Function)**
- Performs well on small datasets.
- Effective for nonlinear prediction problems.

### 4. K-Nearest Neighbors (KNN)

- Distance-based regression algorithm.
- Simple and interpretable.
- Makes predictions using neighboring observations.

---

## Exploratory Data Analysis (EDA)

### Key Observations

- **Load** showed a strong positive correlation with **Wear Rate**.
- **Load** significantly influenced **Coefficient of Friction (COF)**.
- Increasing **TiC content** reduced Wear Rate.
- TiC reinforcement improved overall tribological performance.
- Load was identified as the most influential process parameter.

---

## Evaluation Metrics

The following metrics were used to evaluate model performance:

| Metric | Description |
|----------|------------|
| MAE | Mean Absolute Error |
| RMSE | Root Mean Square Error |
| R² Score | Coefficient of Determination |
| MAPE | Mean Absolute Percentage Error |

---

# Results

## Wear Rate Prediction Performance

| Model | MAE | RMSE | R² Score | MAPE (%) |
|---------|---------|---------|---------|---------|
| ANN | 0.1056 | 0.1316 | 0.6497 | 11.31 |
| Random Forest | 0.0799 | 0.1004 | 0.7959 | 10.06 |
| KNN | 0.0855 | 0.0967 | 0.8106 | 10.70 |
| SVR | 0.0592 | 0.0742 | **0.8887** | **6.24** |

### Best Model for Wear Rate Prediction

**Support Vector Regression (SVR)** achieved the highest prediction accuracy with:

- **R² Score = 0.8887**
- **MAPE = 6.24%**

---

## Coefficient of Friction (COF) Prediction Performance

| Model | MAE | RMSE | R² Score | MAPE (%) |
|---------|---------|---------|---------|---------|
| ANN | 0.000871 | 0.001349 | **0.9619** | **2.79** |
| Random Forest | 0.002805 | 0.003176 | 0.7888 | 8.41 |
| SVR | 0.002201 | 0.002776 | 0.8387 | 6.44 |
| KNN | 0.003169 | 0.003671 | 0.7177 | 9.53 |

### Best Model for COF Prediction

**Artificial Neural Network (ANN)** achieved the highest prediction accuracy with:

- **R² Score = 0.9619**
- **MAPE = 2.79%**

---

## Key Findings

- **SVR** achieved the highest accuracy for **Wear Rate prediction**.
- **ANN** achieved the highest accuracy for **COF prediction**.
- Machine Learning models successfully captured the complex nonlinear relationships between process parameters and tribological responses.
- ML-based prediction can significantly reduce the number of experimental trials required.
- Increasing **TiC reinforcement** improves wear resistance under lubricated sliding conditions.
- Load was identified as the dominant factor affecting both Wear Rate and COF.

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Computation |
| Matplotlib | Data Visualization |
| Scikit-Learn | Machine Learning Models |
| Jupyter Notebook | Model Development & Analysis |

---

## Project Structure

```text
├── Analysis_report.ipynb
├── PPT.pdf
├── Dataset.csv
├── README.md
└── requirements.txt
```

---

## Conclusion

This study demonstrates the effectiveness of Machine Learning techniques in predicting the tribological behavior of Cu–Gr–TiC composites.

Among all evaluated models:

- **SVR** was the most reliable model for Wear Rate prediction.
- **ANN** delivered exceptional performance for COF prediction.

The developed framework can support rapid material design, performance optimization, and reduction of costly experimental investigations.

---

## References

1. **Ankit et al. (2023)** – Prediction of Tribological Performance of Cu–Gr–TiC Composites Based on Response Surface Methodology and Worn Surface Analysis.

2. **Huifeng Ning et al. (2023)** – Modeling and Prediction of Tribological Properties of Copper/Aluminum–Graphite Self-Lubricating Composites using Machine Learning Algorithms.

3. **Ankit et al. (2023)** – Synergetic Influence of TiC and Graphite Particles on Tribological Performance of Cu-Based Composites Prepared by Flake Powder Metallurgy.




