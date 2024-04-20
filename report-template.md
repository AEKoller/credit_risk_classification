# Module 12 Report Template

#The purpose of this analysis was to use loan data to determine whether a loan is healthy (0) or high-risk (1). The data included information on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was the loan status, with 0 indicating a healthy loan and 1 indicating a high-risk loan.

The machine learning process involved the following stages:

Reading the data from a CSV file into a Pandas DataFrame
Separating the features (X) and the target variable (y)
Splitting the data into training and testing sets using train_test_split
Creating a logistic regression model using the training data
Making predictions on the testing data using the fitted model
Evaluating the model's performance using a confusion matrix and classification report
The main algorithm used in this analysis was LogisticRegression from the scikit-learn library.

## Results

- The overall accuracy is very good at 99%. This was calculated by adding the true positives against the true negatives, and subtracting by the total number of samples.

- The model's precision on healthy loans was very good, with a 100% accuracy for predicting healthy loans. The model's prediction on high-risk loans was not as good, but still quite adequate at 84% succesful prediction rate.

- The model's ability to identify true positives was also very good for both healthy (.99) and high-risk loans (.94). 

- Finally, the F1-Score (a harmonic mean between precision and recall) was perfect for healthy loans, and adequate for high-risk loans

## Summary

The logistic regression model performed very well in predicting healthy loans, with perfect precision and a high recall of 0.99. For high-risk loans, the model had a lower precision of 0.84 but a high recall of 0.94. The overall accuracy of the model was 0.9926.

The model's performance is generally good, especially in identifying healthy loans. However, the precision for high-risk loans is lower, which means that the model may classify some healthy loans as high-risk. Depending on the specific requirements and risk tolerance of the client, this level of performance may or may not be acceptable.

If the client prioritizes minimizing false positives (incorrectly classifying healthy loans as high-risk), then further improvements to the model might be necessary. However, if the main concern is identifying as many high-risk loans as possible (maximizing recall for high-risk loans), then the current model's performance may be sufficient.