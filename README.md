# Unit-11-Risky-Business


Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.
In this assignment you will build and evaluate several machine learning models to predict credit risk using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so you will need to employ different techniques for training and evaluating models with imbalanced classes. You will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. Resampling
2. Ensemble Learning



Resampling
Use the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data.
To begin:


Read the CSV into a DataFrame.


Split the data into Training and Testing sets.


Scale the training and testing data using the StandardScaler from sklearn.preprocessing.


Use the provided code to run a Simple Logistic Regression:

Fit the logistic regression classifier.
Calculate the balanced accuracy score.
Display the confusion matrix.
Print the imbalanced classification report.



Next you will:


Oversample the data using the Naive Random Oversampler and SMOTE algorithms.


Undersample the data using the Cluster Centroids algorithm.


Over- and undersample using a combination SMOTEENN algorithm.


For each of the above, you will need to:


Train a logistic regression classifier from sklearn.linear_model using the resampled data.


Calculate the balanced accuracy score from sklearn.metrics.


Display the confusion matrix from sklearn.metrics.


Print the imbalanced classification report from imblearn.metrics.


Use the above to answer the following questions:

Which model had the best balanced accuracy score?




Which model had the best recall score?




Which model had the best geometric mean score?


Ensemble Learning
In this section, you will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. You will use the Balanced Random Forest Classifier and the Easy Ensemble Classifier. Refer to the documentation for each of these to read about the models and see examples of the code.
To begin:


Read the data into a DataFrame using the provided starter code.


Split the data into training and testing sets.


Scale the training and testing data using the StandardScaler from sklearn.preprocessing.


Then, complete the following steps for each model:


Train the model using the quarterly data from LendingClub provided in the Resource folder.


Calculate the balanced accuracy score from sklearn.metrics.


Display the confusion matrix from sklearn.metrics.


Generate a classification report using the imbalanced_classification_report from imbalanced learn.


For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.


Use the above to answer the following questions:


Which model had the best balanced accuracy score?


Which model had the best recall score?


Which model had the best geometric mean score?


What are the top three features?



Hints and Considerations
Use the quarterly data from the LendingClub data provided in the Resources folder. Keep the file in the zipped format and use the starter code to read the file.
Refer to the imbalanced-learn and scikit-learn official documentation for help with training the models. Remember that these models all use the model->fit->predict API.
For the ensemble learners, use 100 estimators for both models.
