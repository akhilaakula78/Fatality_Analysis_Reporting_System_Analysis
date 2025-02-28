# FARS Analysis Project

## Overview
This project analyzes the **Fatal Accident Reporting System (FARS)** dataset using **Apache Spark**. The objective is to explore accident severity, identify contributing factors, and build predictive models for accident severity classification and fatality prediction.

## Data Preparation
- Loaded the dataset into **PySpark**.
- Retained key features related to **accident severity, temporal trends, and road conditions**.
- Checked for and handled missing values.
- Applied **one-hot encoding** to categorical features for modeling.

## Exploratory Data Analysis (EDA)
- Generated summary statistics for numerical variables.
- Visualized distributions using **histograms and correlation heatmaps**.
- Identified trends in accident patterns based on time, location, and road conditions.

## Clustering
- Applied **K-Means clustering** to group accidents based on similar characteristics.
- Used the **elbow method** to determine the optimal number of clusters.
- Applied **Principal Component Analysis (PCA)** for visualization.

## Regression Models
- Built models to predict the number of fatalities in an accident.
- Implemented **Linear Regression, Decision Tree Regressor, and Random Forest Regressor**.
- **Random Forest Regressor** outperformed other models with the lowest error rates and highest explanatory power.

## Classification Models
- Categorized accident severity into **Low, Medium, and High**.
- Implemented **Logistic Regression, Decision Tree Classifier, and Random Forest Classifier**.
- **Decision Tree and Random Forest** performed well in predicting the majority class but struggled with class imbalance.

## Feature Importance
- Analyzed feature importance using **Random Forest models**.
- Key factors influencing accident severity included:
  - **Number of persons involved**
  - **Pedestrian involvement**
  - **Collision type**
  - **Weather conditions**

## Conclusion
This analysis provided valuable insights into accident patterns and severity prediction. **Random Forest models** demonstrated strong predictive capabilities, making them suitable for real-world applications in accident prevention and traffic safety improvements. Future enhancements could include:
- **Balancing the dataset to improve classification performance**
- **Exploring deep learning models**
- **Integrating external datasets for better predictions**

## Technologies Used
- **Apache Spark (PySpark)**
- **MLlib (Machine Learning)**
- **Data Visualization (Matplotlib, Seaborn)**
- **Feature Engineering & One-Hot Encoding**
- **Regression & Classification Models**
- **Clustering & PCA**
