# 📊 Telecom Customer Churn Prediction

## 📌 Project Overview

Customer churn is a common problem in the telecom industry. Customers may leave a company because of pricing, poor service, contract type, lack of support, or other factors.

In this project, I built a **Machine Learning model to predict whether a telecom customer is likely to churn or stay** based on customer information, services, contract details, and billing information.

The project follows a complete Machine Learning workflow, starting from data cleaning and analysis and ending with customer churn prediction.

---

## 🎯 Project Objective

The main objective of this project is to:

* Understand customer churn patterns.
* Analyze customer and service-related data.
* Preprocess the dataset for Machine Learning.
* Build a classification model.
* Predict whether a customer is likely to churn.
* Evaluate the performance of the model.
* Identify the features that have a strong influence on predictions.

---

## 🧠 Machine Learning Approach

This is a **Binary Classification** problem.

The target variable is:

| Churn | Meaning                     |
| ----- | --------------------------- |
| `Yes` | Customer is likely to leave |
| `No`  | Customer is likely to stay  |

For Machine Learning, the target is converted into:

```text
No  → 0
Yes → 1
```

### Algorithm Used

**Random Forest Classifier**

Random Forest combines multiple decision trees to make predictions. It works well with different types of customer information and can also provide feature importance.

---

## 📂 Dataset

The dataset contains information about telecom customers, including:

* Customer demographics
* Tenure
* Phone services
* Internet services
* Online security
* Online backup
* Technical support
* Streaming services
* Contract type
* Payment method
* Monthly charges
* Total charges
* Churn status

Important columns include:

```text
customerID
gender
SeniorCitizen
Partner
Dependents
tenure
PhoneService
MultipleLines
InternetService
OnlineSecurity
OnlineBackup
DeviceProtection
TechSupport
StreamingTV
StreamingMovies
Contract
PaperlessBilling
PaymentMethod
MonthlyCharges
TotalCharges
Churn
```

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Processing
   ↓
Train/Test Split
   ↓
One-Hot Encoding
   ↓
Random Forest Classifier
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Feature Importance


## 🔍 Exploratory Data Analysis

The project analyzes different aspects of customer churn using visualizations.

Some of the analysis includes:

* Customer churn distribution
* Churn by contract type
* Churn by internet service
* Monthly charges vs churn
* Customer tenure vs churn

These visualizations help understand patterns in customer behavior.

🛠️ Technologies Used

# Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib

### Development Environment

* JupyterLab
* VS Code

### Version Control

* Git
* GitHub

---

## 📁 Project Structure

```text
telecom-churn-prediction/
│
├── telecom_churn_prediction.ipynb
├── telecom_churn.csv
├── telecom_churn_model.pkl
├── README.md
│
└── images/
    ├── churn_distribution.png
    ├── confusion_matrix.png
    └── feature_importance.png
```

---



## 🤖 Model Training

The project uses a Random Forest Classifier with preprocessing through a Scikit-learn Pipeline.

Categorical features are converted into numerical features using **One-Hot Encoding**.

The dataset is divided into:

```text
80% → Training Data
20% → Testing Data
```

The model is then trained using the training data and evaluated using the testing data.

---

## 📈 Model Evaluation

The model is evaluated using:

### Accuracy

Measures the overall percentage of correct predictions.

### Precision

Measures how many predicted churn customers actually churned.

### Recall

Measures how many actual churn customers were correctly identified.

### F1 Score

Provides a balance between Precision and Recall.

### Confusion Matrix

Shows:

```text
                Predicted
              No Churn   Churn
Actual
No Churn        TN         FP
Churn           FN         TP
```

---

## 🔎 Feature Importance

Random Forest allows us to analyze which features contribute more to the model's predictions.

The project creates a feature importance visualization to understand the important factors associated with the model's churn predictions.

---

## 👤 New Customer Prediction

The trained model can also be used to predict churn for a new customer.

Example:

```text
Customer:
Contract → Month-to-month
Tenure → 2 months
Internet Service → Fiber optic
Monthly Charges → 70.70
Payment Method → Electronic check
```

The model returns:

```text
Churn Probability: XX.XX%
Prediction: Customer is likely to CHURN
```

The actual probability and prediction depend on the trained model and dataset.

## 💡 What I Learned

Through this project, I learned:

* Data cleaning using Pandas
* Handling missing values
* Exploratory Data Analysis
* Data visualization
* Categorical data encoding
* Train-test splitting
* Machine Learning classification
* Random Forest
* Model evaluation
* Confusion Matrix
* Feature importance
* Making predictions for new customers
* Saving a trained Machine Learning model
* Working with JupyterLab
* Uploading projects to GitHub

## 🎓 Project Type

**Machine Learning | Classification | Data Science | Telecom Analytics**

This project demonstrates the complete Machine Learning pipeline from **raw customer data to a working churn prediction model**.
## 👨‍💻 Author

**Rutvik**
AI & Data Science Engineering Student
⭐ If you find this project useful, feel free to explore the code and improve it further.
