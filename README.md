# Telecom Customer Churn Prediction Using Ensemble Learning

## 📌 Project Overview

This project aims to predict customer churn in the telecommunications industry using machine learning classification models. It uses customer subscription records to identify customers who are likely to discontinue their services.

The project implements data preprocessing, categorical feature encoding, class imbalance handling, model training, cross-validation, and performance evaluation.

## 🎯 Objectives

- Predict whether a customer will churn.
- Clean and preprocess the Telco Customer Churn dataset.
- Encode categorical features using OneHotEncoder.
- Handle class imbalance using SMOTE.
- Train and compare Random Forest and XGBoost classifiers.
- Evaluate models using ROC-AUC, accuracy, precision, recall, and F1-score.
- Visualize ROC curves and identify the top 10 important features.

## 📂 Dataset

**Dataset:** IBM Telco Customer Churn

**Source:** [Download the dataset (CSV)](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

The dataset contains telecom customer information, including:

- Customer demographics
- Contract and payment information
- Tenure and monthly charges
- Total charges
- Churn status

**Target variable:** `Churn`

- `Yes` — Customer churned.
- `No` — Customer did not churn.

## 🛠️ Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- imbalanced-learn (SMOTE)
- Google Colab / Jupyter Notebook

## ⚙️ Methodology

### 1. Data Cleaning
- Remove the customer ID column.
- Convert `TotalCharges` to numeric.
- Identify and handle missing values.

### 2. Exploratory Data Analysis
- Analyze churn distribution.
- Explore customer and subscription characteristics.
- Examine class imbalance.

### 3. Data Preprocessing
- Separate features and target variable.
- Split data into training and testing sets.
- Impute missing values.
- Scale numerical features.
- Apply OneHotEncoder to categorical features.

### 4. Class Imbalance Handling
Apply SMOTE to the training data to balance the target classes and reduce the effect of class imbalance.

### 5. Model Training
Train two classification models:

- Random Forest Classifier
- XGBoost Classifier

### 6. Model Evaluation
Evaluate model performance using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- ROC-AUC score
- Stratified 5-fold cross-validation

### 7. Visualization and Feature Importance
- Compare model ROC-AUC scores.
- Plot ROC curves.
- Visualize the top 10 important features using XGBoost feature importance.

## 📊 Results

The project compares Random Forest and XGBoost based on their predictive performance.

| Metric | Random Forest | XGBoost |
|---|---|---|
| Accuracy | To be measured | To be measured |
| ROC-AUC | To be measured | To be measured |
| Precision | To be measured | To be measured |
| Recall | To be measured | To be measured |
| F1-score | To be measured | To be measured |

**Target:** ROC-AUC greater than 0.80.

Actual results will be added after running the notebook. The target is not a guaranteed outcome.

## 📁 Project Structure

```text
telecom-customer-churn-prediction/
│
├── Telecom_Customer_Churn.ipynb
├── README.md
├── requirements.txt
│
└── results/
    ├── roc_curve.png
    ├── feature_importance.png
    └── model_comparison.csv
```

## 🚀 How to Run

### Option 1: Google Colab

1. Open Google Colab.
2. Upload `Telecom_Customer_Churn.ipynb`.
3. Run the installation cell.
4. Execute the notebook cells in order.
5. Review the evaluation metrics and generated plots.

### Option 2: Local Environment

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `Telecom_Customer_Churn.ipynb` and run the cells sequentially.

## 🔍 Key Learning Outcomes

- Data cleaning and feature engineering
- Categorical feature encoding
- Handling imbalanced classification datasets
- Ensemble learning with Random Forest and XGBoost
- Cross-validation and model evaluation
- ROC curve analysis
- Feature importance interpretation
- Reproducible machine learning workflows

## ⚠️ Limitations

- Model performance depends on dataset quality and selected features.
- SMOTE may not always improve predictive performance.
- Feature importance indicates model influence, not causation.
- Results on this dataset may not generalize to other telecom providers.

## 👩‍💻 Author

**Shamiha Jahan**

GitHub: [@shamiha17](https://github.com/shamiha17)

## 📜 Acknowledgements

Thanks to IBM for providing the Telco Customer Churn dataset and to the open-source Python machine learning community for the tools used in this project.
