
# Heart Disease Prediction Project

## Overview
The Heart Disease Prediction project is a machine learning classification task aimed at predicting the risk of heart disease in patients based on various health indicators. This project leverages a dataset containing several health-related features and uses machine learning algorithms to classify whether an individual has heart disease or not. The primary goal is to build a predictive model that can help in early diagnosis and potentially guide medical intervention.

## Dataset Description
The dataset used in this project consists of several features commonly associated with heart health. Here is a brief explanation of each feature:

1. **Age**: Age of the individual in years.
2. **Sex**: Gender of the individual (1 = male, 0 = female).
3. **CP (Chest Pain Type)**:
   - 0: Typical angina – chest pain related to decreased blood supply to the heart.
   - 1: Atypical angina – chest pain not related to the heart.
   - 2: Non-anginal pain – typically esophageal spasms (non-heart related).
   - 3: Asymptomatic – chest pain not showing signs of disease.
4. **Trestbps (Resting Blood Pressure)**: Resting blood pressure (in mm Hg) on hospital admission; values above 130-140 are typically concerning.
5. **Chol (Serum Cholesterol)**: Serum cholesterol in mg/dl (LDL + HDL + 0.2 * triglycerides); levels above 200 mg/dl are concerning.
6. **Fbs (Fasting Blood Sugar)**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false); above 126 mg/dl indicates diabetes.
7. **Restecg (Resting Electrocardiographic Results)**:
   - 0: Nothing abnormal.
   - 1: ST-T wave abnormality (indicates possible issues).
   - 2: Left ventricular hypertrophy (enlarged main heart chamber).
8. **Thalach (Maximum Heart Rate Achieved)**: The highest heart rate achieved during a stress test.
9. **Exang (Exercise Induced Angina)**: Indicates if the individual experiences angina due to exercise (1 = yes, 0 = no).
10. **Oldpeak**: ST depression induced by exercise relative to rest, indicating heart stress during physical activity.
11. **Slope**: The slope of the peak exercise ST segment.
   - 0: Upsloping – better heart rate response to exercise.
   - 1: Flat – minimal change in heart rate (typical healthy heart).
   - 2: Downsloping – indicates an unhealthy heart.
12. **CA (Number of Major Vessels Colored by Fluoroscopy)**: 0-3; the number of major blood vessels observed during fluoroscopy.
13. **Thal (Thallium Stress Test Result)**:
   - 1, 3: Normal.
   - 6: Fixed defect (past defect now normal).
   - 7: Reversible defect (poor blood movement during exercise).
14. **Target**: Outcome variable indicating the presence (1) or absence (0) of heart disease.

## Project Workflow
The project follows a structured workflow to analyze and build a predictive model:

### 1. Data Loading and Exploration
   - Importing the dataset and libraries (`pandas`, `numpy`, `matplotlib`, `scikit-learn`).
   - Displaying the first few rows and checking for null values.
   - Statistical analysis of each feature.

### 2. Data Preprocessing
   - Handling missing values (if any).
   - Feature scaling and normalization where necessary.
   - Encoding categorical features (e.g., chest pain types, resting ECG results).

### 3. Exploratory Data Analysis (EDA)
   - Visualizing distributions of features (age, cholesterol levels, etc.).
   - Correlation heatmap to understand relationships between features.
   - Visualizing the target distribution to check for class imbalance.

### 4. Model Training and Evaluation
   - **Splitting the Data**: Dividing the dataset into training and testing sets using an 80-20 split.
   - **Model Selection**: Starting with logistic regression as a baseline classifier.
   - **Model Evaluation**: Using evaluation metrics such as accuracy, precision, recall, F1-score, and ROC-AUC score.
   - **Confusion Matrix Analysis**: To understand model performance in terms of true positives, false positives, true negatives, and false negatives.
   - **ROC Curve Analysis**: To visualize the trade-off between the true positive rate and the false positive rate.

## Project Dependencies
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `warnings` (to ignore warnings during execution)

You can install these dependencies using:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## Results
- Include a summary of the model's performance on the testing set.
- Discuss any limitations or potential improvements for future work.
- Optionally, provide screenshots of visualizations (correlation matrix, ROC curve) or a link to a deployed web app.
