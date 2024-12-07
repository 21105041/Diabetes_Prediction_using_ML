# Diabetes_Prediction_using_ML
This is a Diabetes prediction project of 768 female patients using Machine Learning models.

## Overview

This project aims to predict diabetes in patients using machine learning models. The dataset includes various medical diagnostic features such as glucose level, blood pressure, BMI, and insulin, which are analyzed and used to train predictive models. The project explores data preprocessing, feature engineering, and model evaluation, making it an excellent example of applying data analytics and machine learning in healthcare.

---

## Dataset

The dataset used is the **Pima Indians Diabetes Database** from Kaggle. It contains diagnostic measurements for 768 female patients, with the target variable indicating whether a patient has diabetes or not.

### Key Features:
- **Pregnancies**: Number of pregnancies.
- **Glucose**: Plasma glucose concentration.
- **BloodPressure**: Diastolic blood pressure (mm Hg).
- **SkinThickness**: Triceps skinfold thickness (mm).
- **Insulin**: 2-Hour serum insulin (mu U/ml).
- **BMI**: Body mass index.
- **DiabetesPedigreeFunction**: Family diabetes history.
- **Age**: Age of the patient.
- **Outcome**: Indicates diabetes presence (1 = Yes, 0 = No).

---

## Project Workflow

### 1. **Data Preprocessing**
- Handled missing or zero values in critical columns using imputation techniques.
- Addressed outliers through log transformations and normalization.
- Performed Z-score normalization for numerical features.

### 2. **Feature Engineering**
- Created new features:
  - `BMI_Category` (Normal, Overweight, Obese)
  - `Glucose_Category` (Low, Normal, High)
  - Interaction terms such as `Glucose x BMI` and `Age x Pregnancies`.
- Segmented `Age` into bins (Young, Middle-aged, Elderly) to identify trends.

### 3. **Data Visualization**
- Explored distributions and relationships using:
  - Pair plots
  - Heatmaps
  - Box plots and violin plots for comparisons based on diabetes outcome.

### 4. **Model Building**
Used various machine learning models:
- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting**
- **XGBoost**
- **SVM**
- **Voting Classifier** (ensemble of multiple models)

### 5. **Evaluation**
Metrics calculated:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC Score**

**Best Model**: Gradient Boosting with an accuracy of 77% and ROC-AUC score of 83%.

### 6. **Class Imbalance Handling**
- Implemented **SMOTE** (Synthetic Minority Oversampling Technique) and adjusted class weights to address imbalance in the outcome variable.

---

## Insights

1. **Glucose** and **BMI** showed the strongest correlation with diabetes, while features like **Blood Pressure** and **Skin Thickness** had a weaker association.
2. Feature engineering and interaction terms enhanced model performance, highlighting the importance of derived attributes.
3. Addressing class imbalance through SMOTE improved model fairness but did not drastically change performance metrics.

---

## Technical Skills Demonstrated
- Data preprocessing (handling missing values, normalization, and transformations).
- Feature engineering and interaction term creation.
- Machine learning model training, evaluation, and tuning.
- Visualization using libraries like **Matplotlib** and **Seaborn**.
- Handling class imbalance with techniques like **SMOTE**.
- Interpretation of classification metrics for healthcare applications.

---

## How to Use This Repository

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/diabetes-prediction.git
   cd diabetes-prediction

