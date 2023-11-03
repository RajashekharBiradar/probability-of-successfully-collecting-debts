# probability-of-successfully-collecting-debts

# Problem Statement
In the realm of debt collection, the ability to discern which accounts are statute-barred—thus potentially unrecoverable—holds immense significance. This project endeavors to develop a sophisticated machine-learning model aimed at accurately predicting the probability of successfully collecting debts by meticulously examining the statute-barred status of each account.
Given a dataset encompassing a multitude of attributes including original creditor information, account IDs, current balances, purchase dates, and a wealth of other pertinent features, the objective is to construct a predictive model that excels in identifying accounts where the statute barred status may influence the likelihood of debt retrieval.
The focal point of this endeavor centers on the IsStatBarred field, which serves as the pivotal target variable for classification. 



 # Introduction
 Using Machine Learning to forecast the probability of successfully collecting debts by analyzing statute-barred status
 In the realm of debt collection, the ability to discern which accounts are statute-barred—thus potentially unrecoverable—holds immense significance.
 
 # Defining Project Goals
 This project endeavors to develop a sophisticated machine-learning model aimed at accurately predicting the probability of successfully collecting debts.
 Identify key drivers of  debts collection possibility .
 Develop predictive models to anticipate user responses.
 
 # Why This Matters
 Statute-barred accounts can be a challenge for debt collectors, as they may be unrecoverable due to legal time limits.
In the following slides, we will take you through our project approach, methodology, data analysis plan, expected outcomes, and more.
We invite you to join us on this journey as we explore the intricate interplay of data, user behavior in the realm of driving scenarios.

# Data Preparation
Given a dataset encompassing a multitude of attributes including original creditor information, account IDs, current balances, purchase dates, and a wealth of other pertinent features...

The focal point of this endeavor centers on the 'IsStatBarred' field, which serves as the pivotal target variable for classification.

# Data Dictionary
1.EntityID: Unique identifier for each entry.
2.OriginalCreditor[Redacted]: Name of the original creditor, with sensitive information redacted.
3.AccountID: Unique identifier for the account.
4.CurrentBalance: The current balance of the account.
5.DebtLoadPrincipal: The principal amount of the debt load.
6.BalanceAtDebtLoad: The balance at the time of debt load.
7.PurchasePrice: The price at which the debt was purchased.
8.ProductOrDebtType: Type of product or debt.
9.CollectionStatus: Status of the debt collection
10.IsStatBarred: Indicates if the debt is statute-barred. (target variable)
11.CloseDate: The date when the account was closed.
12. Closure Reason: Reason for closing the account.
13. InBankruptcy: Indicates if the account is involved in bankruptcy.
14. AccountInsolvencyType: Type of insolvency related to the account.
15. CustomerInsolvencyType: Type of insolvency related to the customer.
16. IsLegal: Indicates if legal action has been taken.
17. Interest Rate: Interest rate associated with the debt.
18. LastPaymentAmount: Amount of the last payment made.
19. LastPaymentMethod: Method used for the last payment.
20. NumLiableParties: Number of liable parties associated with the account.
21. CustomerAge: Age of the customer.
22. NumPhones: Number of phone contacts associated with the customer.
23. NumEmails: Number of email contacts associated with the customer.
24. NumAddresses: Number of addresses associated with the customer.

# Data Structure
Rows- 406424
Columns- 22

# Data Cleaning
Clean the data by handling missing values.
Ensure that data is in a usable format for analysis
Get the data type information
Data structure size
No of Columns : 24 nos No of Rows : 406423 nos

# Feature Selection
Review the attributes and select the most relevant ones.
might also create new features that could enhance the predictive power of the model
E.g: By converting the categorical variables into numerical
represenattions using techniques like One-Hot Encoding

# Data Splitting
Splitted the data into training and testing set
train test as 80% and test set as 20%
x_train=((325138, 19),
x_test= (81285, 19), y_train=((325138,)y_test=(81285,)

# Model selection
In terms of accuracy, Random Forest outperforms both Logistic Regression and KNN, achieving the highest accuracy score. If accuracy is your primary metric, Random Forest is the top choice.
Random Forest seems to be the best choice based on the results 
Random Forest can provide feature importance scores, which can help with feature selection and data analysis.

# Model Training
Multiple models were trained, including Random Forest, KNN, and Logistic Regression, to determine the best option for deployment. The results showed that Random Forest had the highest accuracy at 97%, while Logistic Regression and KNN had accuracies of 70% and 93%, respectively. This approach allowed for a more informed decision when selecting a model .

# Model Evaluation
We achieved an accuracy of 97%, precision of 98%, recall of 99%, and an f1 score of 98% after selecting Random Forest as our model. The AUC-ROC curve was 100%. These metrics indicate that our model is performing well and can be considered for further analysis.

# Results
the key performance metrics achieved using the Random Forest model:
Accuracy: 97%
Precision: 98%
Recall: 99%
F1 Score: 98%
AUC-ROC: 100%
Emphasize that these metrics collectively indicate that our model is performing well.

# Conclusion
In conclusion, our project successfully developed a predictive model for Collecting Debts by Analyzing Statute-Barred Status . These results hold valuable implications for optimizing debt collection strategies and enhancing creditor collection engagement.







