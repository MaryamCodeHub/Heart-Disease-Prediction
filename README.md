# Heart Disease Prediction Using Logistic Regression

## Technical Documentation Report

### 1. Introduction
This project focuses on developing a machine learning model to predict the presence of heart disease in individuals based on various medical attributes. Utilizing logistic regression, the model analyzes patient data to determine the likelihood of heart disease, aiming to assist healthcare professionals in early diagnosis and treatment planning.

### 2. Objectives

#### 2.1 Primary Objectives
- Predict the presence of heart disease using patient medical data.
- Enhance diagnostic accuracy through machine learning techniques.
- Provide a reproducible and interpretable model for healthcare analytics.

#### 2.2 Technical Objectives
- Implement data preprocessing techniques, including feature scaling and encoding.
- Train and evaluate a logistic regression model.
- Assess model performance using accuracy, confusion matrix, and classification report.
- Ensure code modularity and clarity for future enhancements.

### 3. Dataset
The dataset used in this project is sourced from the [Heart Disease Prediction Dataset](https://raw.githubusercontent.com/kb22/Heart-Disease-Prediction/master/dataset.csv) on GitHub. It comprises 304 entries with 14 attributes, including:
- **Age**: Age of the patient.
- **Gender**: Sex of the patient (1 = male; 0 = female).
- **ChestPainType**: Type of chest pain experienced.
- **RestingBloodPressure**: Resting blood pressure (in mm Hg).
- **Cholesterol**: Serum cholesterol level (in mg/dl).
- **FastingBloodSugar**: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false).
- **ElectrocardiographicResults**: Resting electrocardiographic results.
- **MaximumHeartRate**: Maximum heart rate achieved.
- **ExerciseInducedAngina**: Exercise-induced angina (1 = yes; 0 = no).
- **DepressionInducedbyExercise**: ST depression induced by exercise relative to rest.
- **Slope**: Slope of the peak exercise ST segment.
- **ColoredVessels**: Number of major vessels colored by fluoroscopy.
- **Thalassemia**: Thalassemia condition (3 = normal; 6 = fixed defect; 7 = reversible defect).
- **target**: Diagnosis of heart disease (1 = disease; 0 = no disease).

### 4. Technology Stack

#### 4.1 Core Technologies
- **Python 3.x**: Primary programming language.
- **Pandas**: Data manipulation and analysis.
- **Scikit-learn**: Machine learning library for model building and evaluation.

#### 4.2 Supporting Libraries
- **StandardScaler**: Feature scaling.
- **train_test_split**: Splitting the dataset into training and testing sets.
- **accuracy_score, confusion_matrix, classification_report**: Model evaluation metrics.

### 5. Model Development Workflow

#### 5.1 Data Preprocessing
- **Column Renaming**: Renamed columns for clarity and consistency.
- **One-Hot Encoding**: Converted categorical variables into numerical format using `pd.get_dummies`.
- **Feature Scaling**: Standardized features using `StandardScaler` to normalize the data.

#### 5.2 Model Training
- **Feature Selection**: Separated features (`X`) and target variable (`y`).
- **Data Splitting**: Divided data into training and testing sets (80% training, 20% testing) using `train_test_split`.
- **Model Initialization**: Initialized logistic regression model.
- **Model Fitting**: Trained the model on the training data.

#### 5.3 Model Evaluation
- **Prediction**: Made predictions on the test data.
- **Accuracy Score**: Calculated the accuracy of the model.
- **Confusion Matrix**: Evaluated the performance of the model in terms of true/false positives and negatives.
- **Classification Report**: Provided precision, recall, f1-score, and support for the model's predictions.

### 6. Conclusion

This project demonstrates the application of logistic regression in predicting heart disease using patient medical data. By following a structured machine learning pipeline, the model achieves reliable performance, offering a valuable tool for early diagnosis.  
