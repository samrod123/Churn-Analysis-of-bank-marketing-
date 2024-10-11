# Churn-Analysis-of-bank-marketing-
                                                  ABSTRACT
In this research a bank marketing campaign dataset from Portugal was used to predict future models and the overall effectiveness 
of bank marketing campaigns in submitting a deposit. The dataset explores a range of features that are associated with social and
economic status of individuals which could be used to predict the outcome of successful deposit. This is applicable in optimizing 
future campaigns to result in more successful outcomes and can be applied globally. The required exploratory data analysis and 
data-preprocessing occurred. Different machine learning models were generated by model training, testing and evaluation. 
This is to determine the most dominant features of the dataset. 

Key words: Logistic regression, support vector machine, KNN-nearest classification, decision tree, random forest, XGBOOST and hyperparameter.

                                             INTRODUCTION
Bank marketing campaigns allow the bank institutions to reach out to clients advertising their products for profit through subscriptions by deposit.
Social and economic factors of the client are taken into consideration which can be beneficial in gaining insights into how it influences subscriptions
by term deposits. Future predictions of bank subscriptions can be made based on findings resulting in more successful outcome of campaigns and key performance 
indicators being achieved.Machine learning is growing and highly applicable to resolve real world problems. In this research a bank marketing campaign dataset 
from Portugal was used to predict future models and the overall effectiveness of bank marketing campaigns in submitting a deposit. The dataset explores a range
of features that are associated with social and economic status of individuals which could be used to predict the outcome of successful deposit. 
This is applicable in wide range and can be applied globally. The required exploratory data analysis occurred.

AIMS
The objective of this research is to identify significant features from the dataset and set predictive model 
for future successful outcome by leveraging machine learning models.

DATASET
A dataset is obtained from the UCI machine learning repository that entails direct marketing campaigns of a Portuguese banking institution. 
The research uses 10% of the raw data, which consists of 4521 instances and 17 features including (16 features and output-variable y).  
The goal is to predict client term subscription (yes/no) to a term deposit (y-variable).
Table 1 shows the dataset features including the y variable.

Table 1: The bank marketing campaign dataset features 
No.	Feature	Data type
1	Age 	Numeric/continuous
2	Job	Categorical
3	Marital	Categorical
4	Education	Categorical
5	Default	Categorical
6	Balance	Numeric
7	Housing	Categorical
8	Loan	Categorical
9	Contact	Categorical
10	Day	Categorical
11	Month	Categorical
12	Duration	Numeric
13	Campaign	Numeric
14	Pdays	Numeric
15	Previous	Numeric
16	Poutcome	Categorical
y	Deposit	Categorical

METHOD
Programming Python
Computer programming python libraries Pandas, NumPy and Skilearn use throughout this research. 

I.	EXPLORATORY DATA ANALYSIS
The features the dataset is explored to identify their influence on the subscription of clients and identify if there were any correlations
between the features that may affect the model building. 

II.	DATA PREPROCESSING
One hot encoding was used to convert categorical values into binary values to ensure effective modelling of the features. 
Oversampling using SMOTE technique.

III.	MODELS
The following machine learning algorithms and ensembles were used to predict the successful term deposit for a given feature, 
to identify best predictor model and which feature is highly influential on the target outcome:
               
a)	K-Nearest Neighbor (KNN) weight 
This is a non-parametric supervised learning classifier that uses the basis that instances of each class is surrounded by instances of the same class. 
The training set of instances is given in feature space and a scalar k.  The unlabelled instance is classified by the most frequent label among the
k-training samples neasrest to that instance. This is measured distance between instances, in this research Euclidean distance was used. 

b)	Logistic regression (LR)
Logistic regression is a discriminative model using the logit function an estimation on the probability the prediction is made. 
In this research the Maximum Likelihood Estimation (MLE) was used.

c)	Random forest (RF)
Random Forests are an ensemble learning model for classification and consist of a high combination of decision trees at training time. 
This improves the classification of a single tree classifier by combining bootstrap aggregating method and randomization in the selection 
of data nodes in the creation of a decision tree. Bootstrap aggregating reduces the variance of a model to overcome issues associated with overfitting the training sets with decision trees.

d)	Naïve Bayes 
Naïve Bayes applies the Bayes Theorem with the condition of naïve independence among predictors. 
One feature does not depend on another feature given the class label. 

e)	Support Vector Machine (SVM) 
The algorithm uses optimal hyperplane to separate class labels into different class labels. 
The binary classification aims to find an optimal classifier function. Linear kernel function facilitated in this research with cost value of 0.1. 

IV DISSCUSION & CONCLUSION

In the observation of the features, managment client job roles, married clients, secondary educated had highest subsciptions to term deposit. 
Clients who were married, secondary-educated, and held management positions had the highest subscription rates to term deposits. 
In contrast, a larger proportion of clients without credit defaults chose not to subscribe.
Clients with housing loans showed lower subscription rates compared to those without, and 
clients with personal loans had the lowest subscription rates, nearing zero. Notably, clients contacted by
cellular phone had the highest subscription rates. The month of May recorded the most term deposit subscriptions, 
while December had the fewest. A significant portion of the outcomes was classified as "unknown," followed by successful pre-campaign outcomes.

The results from the classification reports highlight notable differences in the performance of various machine learning models in predicting term deposit subscriptions. Random Forest demonstrated the highest overall performance, achieving a strong balance between precision (0.93 for class 0 and 0.97 for class 1) and recall (0.97 for class 0 and 0.93 for class 1), with an impressive accuracy of 95%. This suggests that Random Forest is highly effective at minimizing both false positives and false negatives, making it a reliable model for this classification task. Logistic Regression also performed well, with an accuracy of 94%, showing similarly high precision and recall scores, although slightly favoring class 1 predictions. K-Nearest Neighbors (KNN) and Decision Trees performed adequately, with accuracies of 93% and 92%, respectively, indicating that while they are useful, they may not generalise as well as Random Forest or Logistic Regression.

Naive Bayes, on the other hand, displayed the weakest performance, with an accuracy of 87%. Although it balanced precision and recall reasonably well, its lower accuracy indicates a higher rate of misclassification compared to the other models. XGBoost, with its fine-tuned parameters, is expected to perform strongly, likely surpassing the others based on its ability to handle complex patterns and interactions.

Overall, Random Forest stands out as the best-performing model due to its ability to handle both classes effectively, while Naive Bayes shows limitations in its predictive power. XGBoost, once fully evaluated, could potentially outperform the rest, making it a promising candidate for further exploration.The machine learning 





