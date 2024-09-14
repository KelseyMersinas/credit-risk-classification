# Credit Score Machine Learning Analysis

This analysis is set to determine the potential for future bank loan risks associated with individual credit borrowers. Given the data on the borrower can we predict the creditworthiness of the borrower?
The data shows loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status, with loan status being represented by 0 or 1 with a 1 being a default on the loans in that instance.For the status of each loan in the data, there are about 75,000 loans in good standing and 2,500 in default. This is only .03% that have defaulted on their loans. To begin, the data was separated into the features that we would be entering into the model to use to make predictions on future loan status. A regression model was made to make predictions and we can generate a confusion matrix and classification report to analyze the accuracy of the results.

## Results
##### Machine Learning Linear Regression Model:
- **Accuracy**: : at .99 accuracy the model is correctly identifying 99% of samples. 
- - There is a very large percentage of the training data that represents loans in good standing. 


- **Precision**: The model's predictions for borrowers who pay back their loans fully are very accurate, with only 86 false positives out of almost 20,000 borrowers. 
- - The model's precision for predicting defaulting is lower at only 87%, meaning that 13% of the time it predicts the likelihood of defaulting incorrectly.

- **Recall**: the model correctly identifies 95% of the creditors according to the model. The model is more likely to accurately predict the borrowers that do not default, with recall for good standing loans at 100%.

## Summary
This model performs fairly well, but the accuracy of this model is being skewed by the imbalance of the data set. With the majority of the data being creditors that have not defaulted, the model learns that most will not default and applies that to the test data. It is only 87% correct on defaulting predictions and there are still false positives in the data set. While the model is correctly predicting the majority of creditors overall, this could be improved with a scaled data set. 
The majority of creditor will have loans in good standing, so the majority of the predictions will be correct as most predictions all into the good standing category. This and the large size of the data makes the model seem very accurate when using percentages to evaluate it's effectiveness. However, there are less false negatives then false positives which is a good sign that this model could be useful for making predictions but the data it is learning from could be scaled to improve performance. 

