# machine_learning_project-supervised-learning

## Project Outcomes
- Supervised Learning: use supervised learning techniques to build a machine learning model that can predict whether a patient has diabetes or not, based on certain diagnostic measurements.The project involves three main parts: exploratory data analysis, preprocessing and feature engineering, and training a machine learning model. 
### Duration:
Approximately 3 hours and 20 minutes.
### Project Description:
In this projects, you will apply supervised learning techniques to a real-world data set and use data visualization tools to communicate the insights gained from the analysis.

The data set for this project is the "Diabetes" dataset from the National Institute of Diabetes and Digestive and Kidney Diseases 
The project will involve the following tasks:

-	Exploratory data analysis and pre-processing: We will import and clean the data sets, analyze and visualize the relationships between the different variables, handle missing values and outliers, and perform feature engineering as needed.
-	Supervised learning: We will use the Diabetes dataset to build a machine learning model that can predict whether a patient has diabetes or not, using appropriate evaluation metrics such as accuracy, precision, recall, F1-score, and ROC-AUC. We will select at least two models, including one ensemble model, and compare their performance.

The ultimate goal of the project is to gain insights from the data sets and communicate these insights to stakeholders using appropriate visualizations and metrics to make informed decisions based on the business questions asked."

## Conclusions


1. The RandomForestClassifier performs better than the LogisticRegression in most metrics.  It scores higher in ROC area under curve, all f1 metrics except for the negative f1-score (it's tied), 
and has higher precision on negative's and recall on positives.  The LogisticRegression model has higher precision on positives and higher recall on negatives.

2. The most important features for both models are Glucose, BMI, and Age.  The order of importance for the features of both models is almost the same, with Blood Pressure moving from 6th to 4th 
when going from the LogisticRegression to RandomForestClassifier model.

3. Insulin level would have likely been a very important feature for both models if it was included.  A future test could be to drop all rows where Insulin is zero, and try building the same models
to see if they performed better.

4. Between the two models, the RandomForestClassifier should be chosen for predicting diabetes.  Not only does it perform slightly better in almost every metric, it also performs much better in a 
very important metric when diagnosing diseases: True Positive Rate.  By improving the True Positive Rate, you increase the number of patients with diabetes who will be diagnosed properly and treated.

