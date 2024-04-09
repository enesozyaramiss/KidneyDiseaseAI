# KidneyDiseaseAI

Library and Module Imports:

![image](https://github.com/enesozyaramiss/KidneyDiseaseAI/assets/62839938/666fa785-183b-4f53-b9ec-631ba6b46975)

At the beginning of the code, commonly used Python libraries and modules such as pandas, numpy, seaborn, datetime, sklearn, gc, sys, os, matplotlib, pickle, pyodbc, time, tqdm, copy, Path, and statsmodels are imported.
Additionally, specific models and functions are imported from sub-modules like xgboost, statsmodels.api, sklearn_pandas, sklearn2pmml, sklearn.preprocessing, sklearn.pipeline, and sklearn.ensemble.
Data Loading:

A file named "CKD_Preprocessed.csv" is read using pd.read_csv() and loaded into a DataFrame (df).
Data Preparation:

Feature vector (X) and target variable (y) are determined. The target variable is the column "Chronic Kidney Disease: yes".
Data is split into training and test sets using train_test_split().
Creating and Training XGBoost Model:

An XGBoost classifier (XGBClassifier) is instantiated with specific parameters (e.g., max_depth, learning_rate, n_estimators).
The classifier is fitted to the training data using .fit() method.

![image](https://github.com/enesozyaramiss/KidneyDiseaseAI/assets/62839938/b0d87353-636a-4687-83ca-86e3c5f8b5a9)

Model Evaluation:

Predictions are made on the test set using .predict() method.
Accuracy score of the XGBoost model is calculated using accuracy_score() from sklearn.metrics.
Cross-Validation with XGBoost:

Cross-validation is performed using XGBoost's cv() function with specified parameters.
Area Under Curve (AUC) metric is calculated for evaluation.
Feature Importance Plotting:

Feature importance is extracted from the trained XGBoost classifier and plotted using xgb.plot_importance().
ROC Curve Plotting:

Receiver Operating Characteristic (ROC) curve is plotted for model evaluation using metrics.roc_curve() and plt.plot() functions.
Additional Model Evaluation:

AdaBoost, Random Forest, Logistic Regression, Support Vector Machine (SVM), and Gaussian Naive Bayes models are trained and evaluated similarly.
Confusion matrices, precision, recall, accuracy, and ROC curves are generated for each model.
Conclusion:

The code demonstrates the process of loading data, preparing it for modeling, training multiple classifiers, and evaluating their performance using various metrics and visualization techniques. It provides a comprehensive analysis of different machine learning models for the given task of classifying chronic kidney disease.
