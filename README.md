# Introduction_to_Python_Final
README – Heart Disease Prediction Using Decision Tree & Naïve Bayes
1. Project Overview
This project builds and evaluates two machine-learning models—Decision Tree Classifier and Gaussian Naïve Bayes to predict the presence of heart disease using the publicly available Heart Disease Dataset. The evaluation includes Accuracy, Precision, Recall, and F1-Score for each class.
The analysis uses 5-fold cross-validation to ensure fair and stable performance comparison.
2. Dataset
Source: Kaggle – Heart Disease Dataset
Rows: ~1,025
Target Variable: target
•	0 = No Heart Disease
•	1 = Heart Disease Present
Features include: age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal, etc.
3. Preprocessing
•	Load dataset from CSV
•	Separate predictor matrix X and target variable y
•	Standardize features using StandardScaler()
•	Apply 5-fold KFold cross-validation (shuffle=True)
Models Used
        1. Gaussian Naïve Bayes (NB)
        2. Decision Tree Classifier (DT)
4. We have added 5 datavisualization for the dataset
   Heatmap - direction variable is linearly related colour and numbers
   Histoplot - Age Distribution of Patients i.e, Age in years to frequency
   Barchart - Chest pain Vs Heatdisease
   piechart - Heart Disease Vs No Disease
   Scattered plot - Age in Years Vs Max heart rate by Heart disease
6. Evaluation Metrics
Metrics computed for Train and Test sets using cross-validation:
•	Accuracy
•	Precision for class 0 and class 1
•	Recall for class 0 and class 1
•	F1-Score 
7. Results Summary
Naive Bayes (NB)
Mean Train Accuracy: 0.83
Mean Test Accuracy:0.82
Precision (Class 0):0.84
Precision (Class 1):0.81
Recall (Class 0):0.78
Recall (Class 1):0.86
F1 Score :0.82
Decision Tree (DT)
Mean Train Accuracy:1
Mean Test Accuracy:1
Precision (Class 0):1
Precision (Class 1):1
Recall (Class 0):1
Recall (Class 1):1
 F1 Score : 1
8. Interpretation
•	NB typically performs well with fewer parameters and avoids overfitting.
•	DT might show higher training accuracy but lower test accuracy if overfitting occurs.
• F1-Score provides a balanced view between precision and recall, especially useful when classes are imbalanced.
9.	Key Finding
The models effectively identified heart disease risk factors like age, chest pain type (cp), and maximum heart rate, with visualizations confirming class imbalance and clinical correlations that align with known cardiovascular patterns.
10. Limitations
Small dataset size limits generalizability and risks overfitting, especially for Decision Trees; missing values or unhandled outliers in features like cholesterol (chol) could bias results; no external validation on diverse populations ignores demographic biases common in UCI data.
Future work should incorporate larger multi-center datasets, advanced feature selection, ensemble methods like Random Forest, and clinical validation metrics beyond accuracy/precision/recall/F1
11. Conclusion
This project demonstrates the use of Machine Learning classification algorithms to predict heart disease and compares their performance using key evaluation metrics. Cross-validated metrics give a more reliable real-world estimate.

