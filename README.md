# credit_risk_assessment
Analysis of feature selection technique on German credit dataset

## ABSTRACT
<p>The project focuses on feature selection techniques in credit risk dataset with data mining techniques. Data Mining is an automated extraction of hidden knowledge from large amounts of data. The computational complexity of the data mining algorithms increases rapidly as the number of features in the dataset increases. </p>
<p>
Real-world credit datasets have accumulated large quantities of information about clients and their financial and payment history. Feature selection techniques are used on such high dimensional data to reduce the dimensionality by removing irrelevant and redundant features to improve the predictive accuracy of data mining algorithms. This work aims to study the information gain, gain ratio and chi-square correlation-based feature selection method to reduce the feature dimensionality. Information gain measure identifies the entropy value of each specific feature. The amount of information gain or entropy is used to decide whether the feature is selected or deleted. The gain ratio applies the normalization technique to information gain using spilt information value. The correlation-based feature selection uses heuristic search strategies to estimate how the features are correlated with the class attribute and how they are important of each other. Experiments were conducted on the German credit dataset available at UCI Machine Learning Repository to reduce the feature dimensionality using these feature selection methods. </p>

See doc-[report.pdf](https://github.com/deepakiron/credit_risk_assessment/blob/main/report.pdf) for detail overview of project
## FEATURE SELECTION TECHNIQUES USED

 1. information gain
 2. gain ration
 3. chi-sqaure correlation

## Machine Learning model used for train and validation
1. Decision Tree
2. Logistic Regression

## conclusion
<p>
We have used 3 feature selection techniques based on it we have reduced the input data 
and run both decision tree and logistic model on this dataset. Based on it below 
is the graph of the output.
</p>

![image](https://github.com/deepakiron/credit_risk_assessment/assets/43108478/cb2f7363-16dd-46d4-a36d-21eae7f4c670)

- From the above figure 1 represents the accuracy of model on different data, accuracy test data while model trained on whole data and datas after selecting subset of features with different feature selection technique.
- we can see even after reduce the dataset with different feature selection technique the accuracy on test data not verying much
- figure 2,4 shows time taken by the model to train on different set of data. we see the after applying feature selection technique we can reduce the data size which are taking less time to traing the model.
- figure 3 shows the size of dataset with and without applying feature selection technique, we see by applying feature selection technique we nearly reduced the size of data by half.

![image](https://github.com/deepakiron/credit_risk_assessment/assets/43108478/8783ea5e-917c-405a-9794-2a4f1491ab6b)

<p>
The above diagram shows the number of features selected to train the model, initially after one-hot encoding we see the dataset has around 60 columns by using the feature selection technique it reduced by at least 50%.
</p>
<p>
In this Project we have applied different Feature Selection Technique in german credit dataset and compare with the without feature selection algorithm with performance and time. We have currently applied mutual information or information gain technique, gain ratio and chi-square correlation to choose selective features from german credit dataset.
We concluded that some of feature does not contribute much information to the feature so we can remove them without losing information and make the model faster.
</p>

