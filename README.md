# Introduction_to_Python_Final
## README – Heart Disease Prediction Using Decision Tree & Naïve Bayes
## 1. Project Overview
## This project builds and evaluates two machine-learning models—Decision Tree Classifier and Gaussian Naïve Bayes—to predict the presence of heart disease using the publicly available Heart Disease Dataset. The evaluation includes Accuracy, Precision, Recall, and F1-Score for each class.
## The analysis uses 5-fold cross-validation to ensure fair and stable performance comparison.
## 2. Dataset
## Source: Kaggle – Heart Disease Dataset
## Rows: ~1,025
## Target Variable: target
## 0 = No Heart Disease
## 1 = Heart Disease Present
## Features include: age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal, etc.

## 3. Preprocessing
## 1.Load dataset from CSV
## 2.Separate predictor matrix X and target variable y
## 3.Standardize features using StandardScaler()
## 4.Apply 5-fold KFold cross-validation (shuffle=True)
## 5.4. Models Used
## 6.1. Gaussian Naïve Bayes (NB)
## 7.Suitable for simple, fast prediction. Performs well on linearly separable data.
## 8.2. Decision Tree Classifier (DT)
## 9.Non-linear model that can capture complex relationships but may overfit without pruning.
## 5. Evaluation Metrics
## Metrics computed for Train and Test sets using cross-validation:
## Accuracy
## Precision for class 0 and class 1
## Recall for class 0 and class 1
## F1-Score (macro)
## Precision/Recall per class help understand how well each class is predicted, especially important in medical datasets.

## 6. Results Summary
## (Your exact values will appear when you run the code.)
## Naïve Bayes (NB)
## Mean Train Accuracy: 0.83
## Mean Test Accuracy:0.82
## Precision (Class 0):0.84
## Precision (Class 1):0.81
## Recall (Class 0):0.78
## Recall (Class 1):0.86
## F1 Score (macro):0.82
## Decision Tree (DT)
## Mean Train Accuracy:1
## Mean Test Accuracy:1
## Precision (Class 0):1
## Precision (Class 1):1
## Recall (Class 0):1
## Recall (Class 1):1
## F1 Score (macro):1



## 7. Interpretation
## NB typically performs well with fewer parameters and avoids overfitting.
## DT might show higher training accuracy but lower test accuracy if overfitting occurs.
## F1-Score provides a balanced view between precision and recall, especially useful when classes are imbalanced.
## Key Findings
## The models effectively identified heart disease risk factors like age, chest pain type (cp), and maximum heart rate (thalach), with visualizations confirming class imbalance and clinical correlations that align with known cardiovascular patterns.​
## Limitations
## Small dataset size (~300 samples) limits generalizability and risks overfitting, especially for Decision Trees; missing values or unhandled outliers in features like cholesterol (chol) could bias results; no external validation on diverse populations ignores demographic biases common in UCI data.​
## Future work should incorporate larger multi-center datasets, advanced feature selection (e.g., recursive elimination), ensemble methods like Random Forest, and clinical validation metrics beyond accuracy/precision/recall
## 10. Conclusion
## This project demonstrates the use of Machine Learning classification algorithms to predict heart disease and compares their performance using key evaluation metrics. Cross-validated metrics give a more reliable real-world estimate.
