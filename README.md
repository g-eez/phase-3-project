# 📊 SyriaTel Customer Churn Prediction

## 🔍 Project Overview

This project focuses on predicting customer churn for **SyriaTel**, a telecommunications provider, by following a full data science lifecycle. It uses a Decision Tree classifier to model churn behavior, uncovers key factors influencing customer decisions, and presents actionable business insights — all documented in a Jupyter Notebook.

## 🧱 Repository Structure

```
.
├── data/                   # Raw dataset
├── .gitignore              # Version control exclusions
├── presentation/           # Final slides summarizing insights
│   └── Presentation.pdf
├── notebook.ipynb          # Full pipeline: cleaning, modeling, evaluation
└── README.md               # Project summary and instructions
```

## 🔄 Project Workflow Summary

### 1. Business Understanding

The project aims to identify which customers are likely to churn and why, providing business value through customer retention strategies and reduced churn-related losses.

### 2. Data Cleaning

The dataset was examined for missing values and inconsistencies. Only essential columns for analysis were cleaned to maintain accuracy.

### 3. Exploratory Data Analysis (EDA)

Key behavioral variables such as charges, service usage, and subscription plans were visualized and compared between churned and retained customers.

### 4. Feature Engineering

New informative features were created, and categorical variables were encoded to suit modeling requirements.

### 5. Model Training

A **Decision Tree Classifier** was chosen for its interpretability. Its performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC

### 6. Calibration

A calibrated classifier was implemented to improve the reliability of churn probability scores, ensuring better decision-making on thresholds.

### 7. Feature Interpretation

The top 8 features influencing churn were ranked using the model's built-in feature importance scores and visualized in a horizontal bar plot.

### 8. Business Recommendations

Recommendations were developed strictly from model results and feature visualizations — no assumptions or speculative insights were used.

## ✅ Final Model Performance (Calibrated)

| Metric    | Score  |
|-----------|--------|
| Accuracy  | 0.9685 |
| Precision | 1.0000 |
| Recall    | 0.7835 |
| F1 Score  | 0.8786 |
| ROC AUC   | 0.8763 |

## 📈 Top Churn Predictors

The top 8 features identified as most influential in determining churn included:

- Total charge
- Customer service calls
- Voice mail plan
- Total international charge
- Total international calls
- International plan
- Total night minutes
- Account length

These were visualized in a descending feature importance bar chart and used to support every business insight.

## 📌 Business Recommendations

Based on validated model results:

- **High Charges → Churn Risk**: High-spending customers are most likely to churn. Consider loyalty discounts.
- **Customer Support Calls → Frustration Indicator**: Users who contact support often tend to churn. Improve service quality.
- **Plans Matter**: Absence of voicemail or international plans is a churn predictor — consider promotional bundles.
- **Usage Behavior**: Night and international minute usage patterns can guide retention offers.

All conclusions are supported by model outputs and data exploration — no assumptions are made.

## 🗺️ Navigation Instructions

- Open `notebook.ipynb` for a full breakdown of the analysis, modeling, and evaluation steps.
- Open `presentation/Presentation.pdf` for a summary view ideal for stakeholders.
- Review visualizations inline in the notebook for insights into churn behavior.

## 📂 Data Access

The dataset is located in the `data/` directory. It contains anonymized customer attributes and a binary churn label.

## 🧪 Getting Started

To reproduce the project locally, install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

Or install everything via a `requirements.txt` (if included):

```bash
pip install -r requirements.txt
```

## 📽️ Presentation Link

For a visual summary of the project, open:

[`presentation/Presentation.pdf`](./presentation/Presentation.pdf)
