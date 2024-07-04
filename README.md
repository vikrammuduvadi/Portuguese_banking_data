Executable code is in Portuguese_banking_data.git

                                          
                                          **  Findings**
This data set is a result of 17 campaigns that happened over a 2 and a half year time-period between May 2008 and November 2010. Also, the Portuguese bank used a couple of marketing methods

Phone calls to the consumers
Internet online banking
The claim is this data targeted around 69,000 clients with a success rate of around 8%.

As seen above, we identified key set of features to determine if a person would deposit. Some of the features were 0 age
1 job
2 marital
3 education
4 default
5 housing
6 loan
7 contact
8 month
9 day_of_week
10 duration

All of the other features were eliminated to simplify the task of modelling. All of the categorical features were encoded by one hot encoding before using pipeline to transform and fit the data.
4 different classification methods KNN, Decision Tree, Logistic Regression, and SVM were used. They were found to operate with an accuracy score of around 90%.
Again tuning of hyper parameters was performed to optimize the scores with the use of GridSearch CV. KNN and Decision Tree's accuracy score slightly went up.
Thus with these objectives in mind we are able to clearly determine if a client would make deposits in the bank or not. 
We have all of the parameters to know which client to target to maximie the chances of acceptance.

**By comparing the four classifiers, here are the basic observations**
KNN takes the lowest amount of time
SVM takes the highest amount of time
Decision tree has a 100% training accuracy but the accuracy drops on the testing data
However an average accuracy rate of 90% was found on the testing data across all the classifiers
Logistic regression takes the lowest amount of time and is useful for simpler cases
For KNN, despite increasing the n_neighbors the increase in percentage is very little. Hence we run the risk of over-fitting.
Like-wise, increasing the max_depth increases the accuracy percentage but not by a lot, hence we run the risk of over-fitting.
