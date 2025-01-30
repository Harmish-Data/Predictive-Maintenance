# Predictive Maintenance using Machine Learning

## Project Overview

This project focuses on predictive maintenance using machine learning models to identify potential failures in industrial machines. By analyzing sensor data, we can proactively detect machine failures and minimize operational disruptions. The dataset used for this project is the AI4I 2020 Predictive Maintenance Dataset from the UCI Machine Learning Repository.

## Dataset Details

- **Source**: AI4I 2020 Predictive Maintenance Dataset
- **Size**: 10,000 rows, 10 columns
- **Key Features**:
  - Air temperature (K)
  - Process temperature (K)
  - Rotational speed (rpm)
  - Torque (Nm)
  - Tool wear (min)
  - Failure Type (target variable)

## Project Workflow

### 1. Data Preprocessing

- Removed unnecessary columns (Product ID, UDI, Target, Type)
- Encoded categorical variables (Failure Type)
- Checked for missing values and handled them accordingly

### 2. Exploratory Data Analysis (EDA)

- Statistical summary of features
- Visualized data distribution using histograms
- Computed correlation matrix with heatmaps

### 3. Data Splitting & Feature Scaling

- Split data into training (80%) and testing (20%) sets
- Standardized feature values using StandardScaler

### 4. Model Training & Evaluation

We trained and evaluated multiple machine learning models:

| Model                | Accuracy |
|----------------------|----------|
| Logistic Regression  | 59.5%    |
| Decision Tree        | 97.3%    |
| Random Forest        | 98.1%    |
| XGBoost              | 98.2%    |

- **Best Model**: XGBoost with an accuracy of 98.2%
- Evaluated models using:
  - Accuracy score
  - Classification report (precision, recall, f1-score)
  - Confusion matrix visualization

### 5. Results Visualization

- Confusion matrices plotted for each model
- Model performance comparison

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - pandas, numpy (data handling)
  - matplotlib, seaborn (visualization)
  - scikit-learn (model training)
  - XGBoost (boosting classifier)
