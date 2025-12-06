# Loan_Approval_Prediction
This is Loan approval prediction project  is done based on the attributes given

A machine learning classification project that predicts whether a loan application should be approved or not based on applicant details such as ApplicantIncome, Education, LoanAmount, etc.

The company seeks **to automate (in real time) the loan qualifying procedure** based on information given by customers while filling out an online application form. It is expected that the development of ML models that can help the company predict loan approval in **accelerating decision-making process** for determining whether an applicant is eligible for a loan or not.

---

# Project Goals

- Clean and preprocess real-world loan data
- Handle missing values and categorical variables
- Perform EDA (Exploratory Data Analysis)
- Remove outliers using IQR method
- Apply feature scaling (MinMaxScaler)
- Train multiple ML models (KNN, Random Forest, Gradient Boosting, etc.)
- Tune hyperparameters to improve accuracy
- Select the best-performing model
- Evaluate using classification metrics

---

# Data Discription

| Feature               | Description                |
| --------------------- | -------------------------- |
| **Gender**            | Male / Female              |
| **Married**           | Yes / No                   |
| **Dependents**        | Number of dependents       |
| **Education**         | Graduate / Not Graduate    |
| **Self_Employed**     | Applicant employment type  |
| **ApplicantIncome**   | Primary income             |
| **CoapplicantIncome** | Secondary income           |
| **LoanAmount**        | Loan amount (in thousands) |
| **Loan_Amount_Term**  | Duration of loan           |
| **Credit_History**    | Past credit record         |
| **Property_Area**     | Urban / Rural / Semiurban  |
| **Loan_Status**       | Target variable (Y/N)      |

# EDA & Preprocessing Steps
Performed EDA including:
- Distribution plots
- Boxplots for outliers
- Correlation heatmap
- Loan approval trends by gender, education, property area, etc.

Pre-processing :
- Handle missing values
- Converting Categorical features to numerical
- Outlier Removal
- Feature Scaling

# Models Implemented
Logistic Regression, KN Neighbors, SVM,
Categorical NB, Gaussian NB, Decision Tree, Random Forest

Model evaluation on Accuracy Score, Confusion Matrix, Precision, Recall and F1 Score

| Model                 | Accuracy (%) |
|-----------------------|--------------|
| KN Neighbors          | 80.536913    |
| Random Forest         | 78.523490    |
| Decision Tree         | 75.167785    |
| Gaussian NB           | 72.483221    |
| Categorical NB        | 71.140940    |
| Logistic Regression   | 54.362416    |
| SVM                   | 51.006711    |

# Best Model 

Best model as per accuracy is KNN algorithm. 

Model performance parameters

Best K Value: `1`  
Best Accuracy: `80.54%`

Classification Report

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **False** | 0.80 | 0.85 | 0.82 | 78 |
| **True**  | 0.82 | 0.76 | 0.79 | 71 |

| Metric | Score |
|--------|--------|
| **Accuracy** | 0.81 |
| **Macro Avg (F1)** | 0.80 |
| **Weighted Avg (F1)** | 0.80 |

