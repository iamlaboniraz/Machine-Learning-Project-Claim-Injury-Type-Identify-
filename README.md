 # Machine Learning Project – Claim Injury Type Identification

## Project Overview

This project focuses on building a multiclass machine learning classification pipeline to identify **workers’ compensation claim injury types** using structured claim-related data.

The goal of the project is to support better decision-making by predicting the type of injury associated with a claim based on demographic, employment, injury, and claim-related features.

This project was developed as part of my machine learning coursework at **NOVA IMS – Information Management School, Lisbon**.

---

## Problem Statement

Workers’ compensation claim datasets often contain large volumes of information related to employees, injuries, claims, and case outcomes. Manually identifying injury categories can be time-consuming and inconsistent.

This project aims to answer:

> Can machine learning models classify workers’ compensation claim injury types using structured claim data?

The classification pipeline can help support:

- Faster claim categorization
- Improved decision-making
- Better understanding of injury patterns
- More consistent claim analysis
- Data-driven support for insurance and compensation workflows

---

## Dataset Description

The project uses a large-scale workers’ compensation claims dataset containing:

- **593,471 records**
- **33 features**
- Claim-related variables
- Injury-related variables
- Demographic information
- Employment-related attributes
- Missingness indicators and engineered features

The dataset required preprocessing, feature engineering, anomaly filtering, and model evaluation before selecting the final classification model.

---

## Project Workflow

The project followed an end-to-end machine learning workflow:

1. Data understanding
2. Data cleaning
3. Missing value treatment
4. Anomaly detection and filtering
5. Feature engineering
6. Train-test splitting
7. Model training
8. Cross-validation
9. Model comparison
10. Final model selection
11. Performance evaluation

---

## Data Preprocessing

Data preprocessing was performed to improve data quality and prepare the dataset for classification.

Key preprocessing steps included:

- Standardizing missing values
- Handling incomplete or inconsistent records
- Filtering anomalous records
- Preparing categorical and numerical variables
- Creating domain-specific features
- Creating missingness indicators
- Ensuring data consistency before model training

Approximately **3.28% anomalous records** were filtered to improve dataset reliability.

---

## Feature Engineering

Feature engineering was used to create more informative predictors for injury type classification.

Engineered features included:

- Demographic-based indicators
- Injury-related indicators
- Employment-related features
- Missingness indicators
- Domain-specific claim attributes

These features helped improve model performance and made the dataset more suitable for supervised learning.

---

## Models Used

Several machine learning models were trained and compared:

- **Logistic Regression**
- **Random Forest**
- **XGBoost**

The models were evaluated using repeated cross-validation and classification performance metrics.

---

## Model Evaluation

The models were evaluated using:

- Macro F1-score
- Train/test performance comparison
- Cross-validation performance
- Generalization ability
- Overfitting analysis

A repeated **6-fold cross-validation** strategy with **2 repeats** was used to evaluate model stability and reliability.

---

## Final Model Selection

After comparing the models, **XGBoost** was selected as the final model because it showed the best generalization performance.

Model comparison summary:

| Model | Observation |
|---|---|
| Logistic Regression | Lower performance and limited ability to capture complex patterns |
| Random Forest | Strong training performance but showed signs of overfitting |
| XGBoost | Best generalization performance and selected as the final model |

XGBoost achieved the strongest balance between training and testing performance, making it the most suitable model for this multiclass classification task.

---

## Key Results

The final model selection was based on generalization performance and macro F1-score.

Key observations:

- XGBoost achieved the best generalization performance
- Random Forest showed signs of overfitting
- Logistic Regression performed weaker compared to tree-based models
- Feature engineering and anomaly filtering improved dataset quality
- Macro F1-score was used to better evaluate performance across multiple classes

---

## Business Value

This project demonstrates how machine learning can support claim classification workflows by:

- Reducing manual effort in claim categorization
- Improving consistency in injury type identification
- Supporting faster claim analysis
- Helping organizations understand injury patterns
- Providing a scalable predictive modeling approach for large claim datasets

---

## Repository Structure

```text
.
├── Group_53_Report 2.pdf
├── Group_53_notebook.ipynb
└── README.md
```

---

## File Descriptions

| File | Description |
|---|---|
| `Group_53_Report 2.pdf` | Final project report containing methodology, preprocessing, feature engineering, model comparison, results, and conclusions |
| `Group_53_notebook.ipynb` | Jupyter notebook containing the machine learning pipeline, preprocessing, model training, and evaluation |
| `README.md` | Project documentation and summary |

---

## Tools & Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Machine Learning
- Multiclass Classification
- Model Evaluation

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/iamlaboniraz/Machine-Learning-Project-Claim-Injury-Type-Identify-.git
cd Machine-Learning-Project-Claim-Injury-Type-Identify-
```

Install the required libraries:

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn jupyter
```

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook:

```text
Group_53_notebook.ipynb
```

---

## Requirements

Suggested `requirements.txt`:

```txt
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
jupyter
```

---

## Key Learnings

Through this project, I strengthened my skills in:

- End-to-end machine learning pipeline development
- Multiclass classification
- Data preprocessing
- Missing value handling
- Anomaly filtering
- Feature engineering
- Cross-validation
- Model comparison
- XGBoost modeling
- Overfitting analysis
- Macro F1-score evaluation
- Translating predictive modeling results into practical insights
