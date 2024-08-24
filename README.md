
---

# Predictive Analysis for Fraudulent Transactions


## Overview

This project aims to develop an advanced machine learning model to detect fraudulent transactions in large datasets—a critical need for financial institutions. The model is designed for high precision and recall, reducing financial losses and safeguarding customer trust.

## Project Structure

- **Notebook**: [notebook.ipynb](notebook.ipynb)

## Situation

Financial institutions face increasing risks from fraudulent transactions, leading to significant financial losses and eroding customer trust. To mitigate these risks, we set out to develop a sophisticated machine learning model capable of accurately identifying fraudulent transactions within vast datasets.

## Task

The objective was to build a predictive model with the ability to detect fraudulent transactions with high precision and recall. This involved not only model creation but also comprehensive analysis to interpret the results and develop actionable plans to mitigate fraud. The challenge was to manage a large dataset of over 6 million records while maintaining the model's accuracy, efficiency, and scalability.

## Action

### Data Understanding and Preparation

1. **Problem Definition**: We began by clearly defining the problem statement and understanding the data structure, which included 6,362,620 rows and 10 columns.
2. **Data Import and Conversion**: The dataset was imported and converted to Parquet format to optimize loading times and processing efficiency for large-scale data.
3. **Exploratory Data Analysis (EDA)**: Conducted thorough EDA to understand the distribution, outliers, and correlations within the dataset. This included visualizations using boxplots for outliers and heatmaps for correlations.
4. **Data Preprocessing**: Removed highly correlated features to avoid multicollinearity and applied SMOTE for oversampling the minority class. Various outlier removal techniques were tested, including DBSCAN, Isolation Forest, Local Outlier Factor, and IQR, with the most effective method selected.

### Model Development

1. **Baseline Models**: Developed baseline models using Random Forest, both with and without outliers. Utilized KFold cross-validation and Random Search CV for hyperparameter tuning, ensuring robust model performance.
2. **Neural Network Architecture**: Built a deep neural network using Keras and TensorFlow, designed with over 112,000 parameters. The model was trained extensively, and metrics such as precision, recall, and F1-score were closely monitored.

### Evaluation and Optimization

1. **Model Evaluation**: Evaluated the model’s performance using precision, recall, and F1-score. Adjusted thresholds to maximize precision, a critical metric for the business case.
2. **Hyperparameter Tuning**: Conducted multiple rounds of hyperparameter tuning to refine the model, resulting in improved accuracy and stability.

### Implementation and Insights

1. **Key Findings**: Identified the most important predictors of fraudulent transactions, such as transaction amount, and made informed decisions to remove less significant features.
2. **Preventive Measures**: Proposed real-time monitoring and infrastructure enhancements to detect and prevent fraudulent transactions effectively.

## Result

The project successfully delivered a highly accurate fraud detection model capable of identifying fraudulent transactions with a high degree of precision. The neural network architecture, combined with rigorous data preprocessing and hyperparameter tuning, resulted in a model that could be deployed in real-time to prevent financial fraud. The project also provided actionable insights on how to improve the model further and implement preventive measures in the infrastructure, ensuring long-term protection against fraud.

---
