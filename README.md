Report:
Objective
The goal of this notebook is to understand and predict for a telecommunications company, and the task is to develop a predictive model that can identify customers who are likely to churn (cancel their subscription) based on various features. The company wants to proactively target these customers with retention offers to minimize churn and maximize customer retention predict whether a customer will churn or not.

1. Data Preprocessing:
i)	Handing Missing value- There is no missing Value in this data.
ii)	Categorical to Continuous- There is 4 Categorical column in this data are ‘gender’, ‘contract_type’ , ‘payment method’ and ‘churn’ with the help of label encoding we converted all the categorical values into numerical.
iii)	There is no any duplicate value in this data.



2.EDA (Exploratory Data Analysis):
i) The datatypes and Column names were right and there was 20 rows and 9 columns 
ii)The output column contains categorical values so this particular problem belongs to Classification.
iii) No missing values present in the dataset.
iv) No duplicates rows are present in the dataset.
v) Gender, Contract_type,Payment_method,churn these featues are categorical .
vi) Monthly_charges has a correlation of approximately -0.733 with 'churn'. 
vii)   suggests that as the monthly charges increase, there is a tendency for customers to be less likely to churn.
viii) Total_charges has a correlation of approximately -0.753 with 'churn'.
 ix)  which implies that as the total charges incurred by customers increase, the likelihood of churn decreases.
x) Tenure has a correlation of approximately -0.774 with 'churn'. 
xi)   which indicates that customers with longer tenure (i.e longer duration of service) are less likely to churn.
xii) Contract_type has the strongest correlation with 'churn' at approximately -0.841. 
xiii)   suggests that customers who have an annual contract type are significantly less likely to churn           compared to those with a monthly contract type..
            
Categorical to Continuous- There is 4 Categorical column in this data are ‘gender’, ‘contract_type’ , ‘payment method’ and ‘churn’ with the help of label encoding we converted all the categorical values into numerical.

Model building
 In this classification problem to check the model performance three machine learning algorithm are used which is logistic regression ,Knn Classifier and  Decision Tree. 
•	Dependent variable - churn 
•	Independent variable –   age, gender, monthly_charges, total_charges, tenure etc.
Accuracy for the model is good using logistic regression and decision tree as compare to Knn Classifier.
Accuracy:
Logistic Regression:
Accuracy for Testing = 100
Accuracy for Training = 100
Model Evaluation 
In this project two evaluation matrices are used which is given below.
1)	In Knn Classifier
a)	grid search cv (gscv)
b)	randomized search cv(rscv)
2)	In decision tree
a)	decision gscv
b)	decision rscv

When we used evaluation metrices then accuracy became decreasing so , we decided to built final model on logistic regression .

The final model's build on logistic regression because its impeccable accuracy, precision, recall, and F1-score on the given dataset showcase its exceptional performance. It successfully classified all instances, providing reliable predictions and demonstrating its effectiveness in accurately distinguishing between the two classes.
