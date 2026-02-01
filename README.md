Task Title

Credit Card Fraud Detection using Random Forest

Tools & Technologies Used:

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

Joblib

Dataset

File Used: creditcard.csv

Description:
The dataset contains credit card transactions made by European cardholders.
It includes numerical features obtained after PCA transformation and a target column named Class, where:

0 → Legitimate transaction

1 → Fraudulent transaction

The dataset is highly imbalanced, with very few fraud cases compared to non-fraud cases.

Objective:

The objective of this task is to:

Detect fraudulent credit card transactions

Handle imbalanced data effectively

Apply ensemble learning using Random Forest

Evaluate the model using appropriate metrics such as Precision, Recall, and F1-score

Identify important features contributing to fraud detection

Methodology:
The methodology for this task began with loading the credit card fraud dataset and performing exploratory analysis to understand its structure and the severe class imbalance. The data was preprocessed by separating features from the target column (Class). A stratified train-test split was applied to maintain the proportion of fraud cases in both sets. Initially, Logistic Regression was considered, but Random Forest was chosen due to the dataset size and imbalance. The Random Forest model was trained with multiple decision trees to improve generalization and reduce overfitting. Model performance was evaluated using Precision, Recall, and F1-score, which are suitable for imbalanced data. A confusion matrix was created to visualize predictions, and feature importance analysis identified key variables influencing fraud detection. Finally, the trained Random Forest model was saved using Joblib for future use and deployment. 

 Model Evaluation:

model	precision	recall	f1
1	Random Forest	0.983051	0.794521	0.878788
0	Logistic Regression	0.081886	0.904110	0.150171


 precision    recall  f1-score   support

           0     0.9996    1.0000    0.9998     36789
           1     0.9831    0.7945    0.8788        73

    accuracy                         0.9996     36862
   macro avg     0.9913    0.8972    0.9393     36862
weighted avg     0.9996    0.9996    0.9995     36862

Conclusion:

This task provided hands-on experience in building a real-world fraud detection system. By applying Random Forest and focusing on appropriate evaluation metrics, the model effectively identified fraudulent transactions despite severe class imbalance. This task enhanced understanding of ensemble learning and practical machine learning workflows.
