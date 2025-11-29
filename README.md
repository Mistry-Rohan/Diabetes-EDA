# Diabetes-EDA
This repository contains EDA on Diabetes Dataset. Along with EDA, Logistic Regression and Random Forest Models are applied and compared as well for prediction purpose.

The repository includes the dataset file named "diabetes.csv" and the analysis python file name "rohan_041081134". 

## Problem Statement:

One of the widespread health conditions globally is diabetes, with a growing number of individuals affected. The precise origin of diabetes remains unknown, though scientists theorize that a combination of environmental factors, lifestyle choices, and genetic predisposition plays a substantial role in its development.

Several years ago, a study was carried out on American Pima tribe, which are also known as Pima Indians. The study showed that women of this tribe had an early risk of developing diabetes. While preparing the dataset, a number of restrictions were placed on which data is to be selected. Specifically, data chosen was of around the female patients who were atleast 21 years old and descended from Pima Indians.

## Dataset Information:

**Pregnancies**: Number of times pregnant

**Glucose**: Plasma glucose concentration a 2 hours in an oral glucose tolerance test

**Blood pressure**: Diastolic blood pressure (mm Hg)

**SkinThickness**: Triceps skinfold thickness (mm)

**Insulin**: 2-Hour serum insulin (mu U/ml) test

**BMI**: Body mass index (weight in kg/(height in m)^2)

**DiabetesPedigreeFunction**: A function that scores likelihood of diabetes based on family history

**Age**: Age in years

**Outcome**: Class variable (0: the person is not diabetic or 1: the person is diabetic)

## Methodology and Workflow
### 1. Data Exploration & Quality Assessment
- Loaded and inspected the dataset in Python.
- Conducted statistical analysis to examine data distributions.
- Identified missing values using pandas library functions
- Detected outliers using the IQR method. 

### 2. Feature Engineering & Selection
- Performed correlation analysis to identify influential predictors.
- Created new derived metrics to improve predictive power.

### 3. Data Preprocessing
- Standardized/scaled numerical features for model compatibility.
- Split data into training and testing sets using stratified sampling for balanced representation.

### 4. Modeling Approach
- Implemented multiple classification algorithms (Logistic Regression, Random Forest, SVM).
- Performed hyperparameter tuning (Grid Search) to optimize model performance.

### 5. Model Evaluation
- Assessed models using accuracy, precision, recall, and F1-score.

### 6. Interpretation & Recommendations
- Generated actionable insights based on model results to support early diabetes risk identification.

