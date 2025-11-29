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


## Observations
- There is very weak correlation between Glucose, SkinThickness and DiabetesPedigreeFunction. 
- SkinThickness and Glucose seem to have negative direction.
- Moreover, DiabetesPedigreeFunction and Glucose also seem to have a negative direction.
- There seems to presence of outliers.
- The values are overlapped in the plot of all three variables and therefore simple models cannot be used to predict the outcomes based on any two variables from all the three variables.
- Many zero values are also observed for Glucose and SkinThickness.

  ### Scatter Plot between Insulin and Glucose
- Glucose values less than 40 are rarely seen. There are many zero values found for insulin when range of Glucose values are between 50 and 200.
- In general the realation between Insulin and Glucose seems to be in positive direction and the form appears to be linear.
- There is a presence of outliers.
- Strength is weak.

### Correlation Matrix for all the variables
- No two variables have a high corelation or even near 1 which means there are no duplicate values.
- Majority of the correlations are weak correlations.
- There are few intersting moderate correlations observered
  1. Age and pregancies are moderately correlated with r=0.55
  2. Insulin and SkinThickness are moderately correlated with r=0.47
  3. BMI and SkinThickness are moderately correlated with r=0.39
  4. Insulin and Glucose are moderately correlated with r=0.33
   
### Predictive Machine Learning Models
- The accuracy of the Logistic Regression Model on the train set is 76% and the accuracy on the test set is 75%.
- The number of True Positives are 60 and the number of True Negatives are 53.
- The accuracy of the random forest model on train set was 82% and that with the test set was 79%.
- The Number of True Positives were 56 and the number of True Negatives were 63.
- The Random Forest Model has better accuracy on both training and test data compared to Logistic Regression Model. However, the number of Type 2 error in Random Forest Model is found to be slightly higer than the Logistic Regression Model.
