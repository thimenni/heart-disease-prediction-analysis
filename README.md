# Heart Disease Prediction using Machine Learning

## Project Overview
This project focuses on building a machine learning model to predict the presence of heart disease based on patient medical data. The dataset used is the **Heart Disease Dataset: Comprehensive** provided by IEEE DataPort, which combines several heart disease datasets including Cleveland, Hungarian, Switzerland, Long Beach VA, and Statlog.

## Dataset Description

- **Total Instances:** 1,190
- **Number of Features:** 11
- **Task Type:** Binary Classification
- **Target Variable:** (1 indicates presence of heart disease, 0 indicates absence)

For a detailed explanation of dataset and all features, please refer to the original dataset description available at the [source link](https://ieee-dataport.org/open-access/heart-disease-dataset-comprehensive).

### Features Used:
- `age`: Age of the patient
- `sex`: Gender (1 = male, 0 = female)
- `cp`: Chest pain type (0-3)
- `trestbps`: Resting blood pressure
- `chol`: Serum cholesterol (mg/dl)
- `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- `restecg`: Resting electrocardiographic results (0-2)
- `thalach`: Maximum heart rate achieved
- `exang`: Exercise induced angina (1 = yes, 0 = no)
- `oldpeak`: ST depression induced by exercise relative to rest
- `slope`: The slope of the peak exercise ST segment
- `target`: 1 indicates presence of heart disease, 0 indicates no disease

## Methodology
1. **Data Preprocessing and Explorary Data Analysis**
   - Handling duplicates, missing values, invalid values
   - Simple statistics 
   - Detect and remove outliers with Interquartile Range (IQR) method
   - Correlation Analysis 
   - Feature scaling
   - Train-test split

2. **Model Selection**
	 - K-Nearest Neighbors (KNN)
	 - Decision Tree 
   - Logistic Regression
   - Support Vector Machine (SVM)
   - AdaBoost 

3. **Evaluation Metrics**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
   - ROC-AUC Score
   
## Results 
- Best-performing Model: Logistic Regression achieved the highest accuracy of 87% on the test set.
- Key insights from feature importance analysis: 
![5-Importance-Features](https://github.com/thimenni/heart-disease-prediction-analysis/blob/main/results/five_importance_features.png)

Features such as Chest Pain Type, ST Slope, Sex, Fasting Blood Sugar, and Exercise-induced Angina emerged as important predictors in the dataset, significantly contributing to identifying whether a patient has heart disease. This was also evident during Exploratory Data Analysis (EDA) through correlation analysis.
