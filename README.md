# credit-risk-classification

Overview of the Analysis

The purpose of this analysis was to develop machine learning models to predict loan statuses based on financial information provided in a dataset. The dataset contained various features related to loan applications, and the goal was to predict whether a loan would be approved or denied.

The variables we were trying to predict were loan statuses, categorized as either approved or denied. We initially examined the distribution of these statuses using value_counts() to understand the balance between approved and denied loans.

The machine learning process involved several stages:

Data Preprocessing: We imported the dataset, separated it into labels (loan statuses) and features, and split the data into training and testing sets.
Model Selection: We chose logistic regression as our initial model for its simplicity and interpretability.
Model Training: We trained the logistic regression model using the training data.
Model Evaluation: We made predictions using the testing data and evaluated the model's performance using confusion matrix and classification report metrics.

Results

Machine Learning Model 1: Logistic Regression
Accuracy: 0.99
Precision:
Class 0 (Denied Loans): Precision = 1.00, Recall = 1.00, F1 Score = 1.00, Support = 18,759
Class 1 (Approved Loans): Precision = 0.87, Recall = 0.89, F1 Score = 0.88, Support = 625
Macro Average (across both classes):
Precision = 0.94
Recall = 0.94
F1 Score = 0.94
Support = 19,384
Weighted Average (weighted by support):
Precision = 0.99
Recall = 0.99
F1 Score = 0.99
Support = 19,384


Summary

The logistic regression model demonstrates outstanding performance with an accuracy of 99%. It achieves perfect precision and recall for denied loans (class 0), indicating precise identification of all denied loans without any false positives or false negatives. For approved loans (class 1), the model achieves a commendable precision of 87% and a recall of 89%, with an F1 score of 0.88.

Considering the weighted average metrics, which account for the class imbalance in the dataset, the model maintains high precision, recall, and F1 score across both classes. This indicates a robust performance in predicting loan statuses.

In conclusion, the logistic regression model proves to be highly effective in predicting loan statuses based on the provided financial information. Its exceptional accuracy and balanced performance across classes make it a suitable choice for deployment in real-world scenarios. However, continuous monitoring and evaluation are recommended to ensure its performance remains optimal over time.