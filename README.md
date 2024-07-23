**Objective**
The objective of this project is to predict whether a blood donor will donate within a specified time frame using historical data from the Blood Transfusion Service Center.

Data Source
Donor Data: Blood Transfusion Service Center
Dataset Size: 748 donors
Tools Required
Python
Pandas
Logistic Regression
TPOT Library
Process Steps

#Task 1: Inspect the Dataset
Action:
Used shell command to print the first 5 lines of the dataset to understand its structure and contents.

#Task 2: Load the Dataset
Action:
Imported the pandas library.
Loaded the dataset into a DataFrame named transfusion.
Displayed the first few rows to ensure correct loading.

#Task 3: Inspect DataFrame Structure
Action:
Utilized the info() method to print the structure of the DataFrame, providing insights into column types and non-null values.

#Task 4: Rename a Column
Action:
Renamed the column whether he/she donated blood in March 2007 to target for simplicity and clarity.

#Task 5: Print Target Incidence
Action:
Applied value_counts() on the target column to print the incidence proportions, giving insight into the distribution of donation events.

#Task 6: Split the Dataset
Action:
Imported train_test_split from sklearn.model_selection.
Split the data into X_train, X_test, y_train, and y_test, ensuring stratification on the target to maintain distribution consistency.

#Task 7: Use TPOT to Find Best Pipeline
Action:
Imported TPOTClassifier and roc_auc_score.
Instantiated and trained a TPOTClassifier.
Displayed pipeline steps and calculated the AUC score to evaluate model performance.

#Task 8: Check Variance
Action:
Printed the variance of features in X_train to identify any potential high variance features that might need normalization.

#Task 9: Correct for High Variance
Action:

Normalized the feature with the highest variance using log transformation.
Updated both X_train and X_test accordingly.

#Task 10: Train Logistic Regression Model
Action:
Imported LogisticRegression from sklearn.linear_model.
Trained the logistic regression model on the data.
Printed the AUC score to assess model effectiveness.

#Task 11: Sort Models by AUC Score
Action:
Sorted and listed models based on their AUC scores from highest to lowest, facilitating easy comparison of model performance.

**Conclusion**
The project successfully developed a predictive model to forecast blood donations using machine learning techniques. This model aids in optimizing the blood supply chain by improving prediction accuracy, ensuring a balanced supply of blood donations.
