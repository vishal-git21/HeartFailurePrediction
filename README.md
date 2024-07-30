# Heart Failure Prediction

## Overview

This project focuses on predicting the likelihood of heart failure using a variety of machine learning techniques. Heart failure is a serious condition resulting from cardiovascular diseases (CVDs), which are the leading cause of death globally. By leveraging a dataset with various patient attributes, I aim to classify whether a patient is prone to heart failure.

## Dataset

The dataset used in this project is sourced from Kaggle:

- **Dataset Name**: Heart Failure Prediction
- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)

The dataset includes various attributes such as age, sex, chest pain type, blood pressure, cholesterol levels, fasting blood sugar, electrocardiogram results, maximum heart rate, exercise-induced angina, oldpeak, and ST slope.

## Project Steps

1. **Data Loading**: Imported the dataset and examined its structure.
2. **Exploratory Data Analysis (EDA)**: Analyzed data distributions, correlations, and visualized key attributes.
3. **Feature Encoding**: Converted categorical features into numerical values suitable for machine learning models.
4. **Feature Scaling**: Normalized numerical features to improve model performance.
5. **Exogenous Variable Generation**: Added new features to enhance model accuracy:
    - **Age Group**: Categorized age into bins (e.g., 30-40, 41-50).
    - **BP Category**: Categorized blood pressure into stages (e.g., Normal, Elevated).
    - **Cholesterol to Age Ratio**: Ratio of cholesterol to age.
    - **Cholesterol to BP Ratio**: Ratio of cholesterol to blood pressure.
    - **Exercise-Induced Oldpeak**: Product of exercise-induced angina and oldpeak.
    - **ST Slope Value**: Mapped ST slope types to numerical values.
    - **Risk Score**: Computed a risk score based on weighted attributes.
6. **Model Training**: Trained several models, including XGBoost, Gradient Boosting, and Random Forest.
7. **Hyperparameter Tuning**: Optimized model parameters to achieve better performance.
8. **Model Evaluation**: Assessed model performance using metrics such as accuracy, ROC-AUC score, and feature importance visualization.

## Results

The models achieved an accuracy of approximately 90%. The high performance indicates the effectiveness of the chosen models. However, it is noted that a dataset with a greater number of data points could potentially improve model performance further.

## Installation

Clone the repository :

```bash
git clone https://github.com/vishal-git21/HeartFailurePrediction.git
```

## Usage

Run the Jupyter Notebook for a detailed walkthrough of the analysis:

```bash
jupyter notebook PredictingHeartFailure.ipynb
```

## Acknowledgments

- Kaggle for providing the dataset.
- Machine learning libraries such as XGBoost, Gradient Boosting, and Random Forest for model building and evaluation.
