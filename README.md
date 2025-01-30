# Data-Driven Predictive Maintenance: Reducing Downtime in Manufacturing

## Overview

This project focuses on implementing predictive maintenance using machine learning to minimize equipment failures and operational downtime in the manufacturing sector. By leveraging historical maintenance records and sensor data, the project applies advanced ML algorithms to predict failures and optimize maintenance schedules, ultimately improving efficiency and reducing costs.

## Motivation

Traditional maintenance strategies rely on reactive approaches, leading to unexpected failures and financial losses. This project integrates Industry 4.0 concepts, IoT sensor data, and machine learning to create a proactive maintenance solution.

## Dataset

- **Source**: AI4I 2020 Predictive Maintenance Dataset
- **Size**: 10,000 records | 10 features
- **Key Variables**:
  - Air Temperature (K)
  - Process Temperature (K)
  - Rotational Speed (rpm)
  - Torque (Nm)
  - Tool Wear (min)
  - Failure Type (target variable)

## Project Workflow

### 1. Data Preprocessing

- **Cleaning**: Dropped unnecessary columns (Product ID, UDI, Type)
- **Encoding**: Converted categorical Failure Type into numerical labels
- **Feature Scaling**: Standardized numerical features for optimal ML performance

### 2. Exploratory Data Analysis (EDA)

- Statistical insights into feature distribution
- Correlation analysis using heatmaps
- Visualization of failure type occurrences

### 3. Machine Learning Model Implementation

The following models were trained and evaluated:

| Model                | Accuracy |
|----------------------|----------|
| Logistic Regression  | 59.5%    |
| Decision Tree        | 97.3%    |
| Random Forest        | 98.1%    |
| XGBoost              | 98.2%    |

### 4. Results & Findings

- **Best Model**: XGBoost (98.2% accuracy)
- **Confusion Matrix Analysis**: High precision and recall in identifying failure patterns
- **Maintenance Optimization**: The model effectively predicts equipment failures, reducing downtime

### 5. Visualization

- Histograms & KDE plots for feature distribution
- Heatmaps for feature correlation
- Confusion matrices for model evaluation

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - pandas, numpy (Data handling)
  - matplotlib, seaborn (Visualization)
  - scikit-learn, XGBoost (Machine learning)
  - Google Colab (Cloud-based execution)
