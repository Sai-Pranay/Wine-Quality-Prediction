# Wine Quality Prediction

This project involves predicting the quality of wine based on various chemical properties using machine learning techniques. The dataset used for this project is the **Wine Quality Dataset**, which contains both red and white wine data, including several chemical attributes such as acidity, pH, alcohol content, and more.

---

## Overview

The goal of this project is to predict the quality of wine based on its chemical composition. The project uses a dataset containing features like **fixed acidity**, **volatile acidity**, **citric acid**, **residual sugar**, and others to classify the quality of wine on a scale from 0 to 10.

The project applies various data exploration, preprocessing, and machine learning techniques to build an effective model. In particular, the **Random Forest** model has been used for this classification task.

---

## Dataset

- **Source**: UCI Machine Learning Repository
- **Dataset**: The dataset contains 1599 samples of red wine with 12 features each, including:
  - Fixed acidity
  - Volatile acidity
  - Citric acid
  - Residual sugar
  - Chlorides
  - Free sulfur dioxide
  - Total sulfur dioxide
  - Density
  - pH
  - Sulphates
  - Alcohol
  - Quality (target variable)

---

## Features and Columns

- **fixed acidity**: Level of acidity
- **volatile acidity**: Volatility of the acidity
- **citric acid**: Presence of citric acid
- **residual sugar**: Amount of residual sugar
- **chlorides**: Chloride content
- **free sulfur dioxide**: Free sulfur dioxide content
- **total sulfur dioxide**: Total sulfur dioxide content
- **density**: Density of the wine
- **pH**: pH level of the wine
- **sulphates**: Sulphate content
- **alcohol**: Alcohol content in the wine
- **quality**: Target variable indicating wine quality (0-10)

---

## Project Steps

1. **Data Loading**: The dataset is loaded and explored to understand its structure.
2. **Data Exploration**: Visualizations like bar plots are used to investigate relationships between features (e.g., quality vs. volatile acidity).
3. **Data Preprocessing**:
   - Handling missing values
   - Feature scaling and encoding
4. **Model Building**:
   - Various models like **Random Forest** are trained and evaluated using cross-validation techniques.
   - Model evaluation based on accuracy and other metrics like confusion matrix and classification report.
5. **Results**: The trained models' performance is analyzed, and the best-performing model is selected.

---

## Results

- The project evaluates multiple models, and the **Random Forest Classifier** performs best in predicting the quality of wine.
- Evaluation metrics like accuracy, precision, recall, and confusion matrix are used to assess model performance.

---

## Visualizations

- **Quality vs. Volatile Acidity**: The relationship between wine quality and volatile acidity is visualized using a bar plot to understand how these features impact the wine's quality.

```python
fig = plt.figure(figsize = (10,6))
sns.barplot(x = 'quality', y = 'volatile acidity', data = wine)
