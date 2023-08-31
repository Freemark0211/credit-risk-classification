# credit-risk-classification

# Module 20 Challenge


## Synopsis:

	Using data supplied by BootCampSpot of bank customer records determine whether they should be placed into healthy loan or high-risk loan categories.

## Analysis:
-	Using given information of loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts,
	derogatory_marks, total_debt, and loan_status create a model that would accurately predict future
	loan_status given all previously supplied information except for loan status.
  
- 	take given data and split into target(loan_status) and features(all other categories)

-	take this data a separate into training and testing data

-	create a logistic regression model using SciKitLearn using the training data

-	compare the model results to the actual testing data to evaluate accuracy of model

## Results

		      precision    recall  f1-score   support
	
	           0       1.00      0.99      1.00     18765
	           1       0.85      0.91      0.88       619
	
	    accuracy                           0.99     19384
	   macro avg       0.92      0.95      0.94     19384
	weighted avg       0.99      0.99      0.99     19384

 	1. Precision: Percentage of correct positive predictions relative to total positive predictions.

	2. Recall: Percentage of correct positive predictions relative to total actual positives.
	
	3. F1 Score: A weighted harmonic mean of precision and recall. The closer to 1, the better the model.
 	https://www.statology.org/sklearn-classification-report/

## Summary

	 The model overall accurately predicted loan_status based on given data. It was significantly
	 better at predicting healthy loan (0 status) than high-risk (1 status). While the F1 score of .88
	 is still indicates a fairly high accuracy for the high_risk status I would recommend testing other
	 models to see if the accuracy here could be improved. Considering that the bank is most likely more
	 interested in risk abatement. 
