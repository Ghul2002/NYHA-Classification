# NYHA-Classification
## Classification of stages of heart failure. University Exercise

## 1. Data Preparation
Loading data from a CSV file.

Changing the decimal separator from a comma to a period in all numeric columns.

Removing or transforming text columns and those with a large number of missing values.

Imputation of missing values ​​(e.g., median for numbers).

## 2. Data Type Checking and Repair
Converting all predictors to numeric types (float64 or int64).

Ensuring that all column names (features) are of type string.

## 3. Splitting into Training/Test Sets
Extracting the predictors (X) and the target label (y — NYHA_CLEAN).

Splitting into training and test sets (e.g., 80/20), maintaining the class ratio (stratify=y).

## 4. Oversampling SMOTE on the training set
Using SMOTE to balance the classes in the training set so that the model also learns the minority classes.

Checking whether the cardinality of all classes is equal after SMOTE.

## 5. Training the Random Forest classifier
Training the RandomForest model on the balanced training set.

Predicting NYHA classes on the original (unchanged) test set.

## 6. Evaluating model quality
Calculating the accuracy, confusion matrix, and classification report (precision, recall, f1-score for each class).
