**Customer Churn Prediction**
***Project Goal***
The goal of this project is to predict whether a bank customer is likely to leave the bank 
(churn) or continue as a customer. 
To do this, we trained machine learning models using the customer dataset provided. 
These models analyze customer information and try to identify patterns that indicate 
whether a customer may exit. 
Models Used 
For this task, we used Support Vector Machine (SVM), which is a popular machine 
learning algorithm for classification problems. 
Two versions of the model were trained: 
1. Linear Kernel SVM 
This model assumes that the relationship between the features and the target variable is 
mostly linear. 
2. Polynomial Kernel SVM 
This model can capture more complex relationships by allowing non-linear decision 
boundaries. 
Model Results 
Model 
Linear Kernel SVM 
F1 Score 
0.5044 
Polynomial Kernel SVM 0.5649 
The Polynomial Kernel SVM performed better, which suggests that the relationship 
between the customer features and churn is not strictly linear. 
Main Steps in the Project 
1. Data Exploration 
The dataset contained 10,000 customer records with 14 columns. 
2. Data Cleaning 
Some columns were removed because they do not help predict customer churn: 
• RowNumber 
• CustomerId 
• Surname 
3. Data Preparation 
Before training the models, the dataset needed some preprocessing: 
• The target variable was defined as Exited, which indicates whether the customer 
left the bank. 
• Categorical variables such as Geography and Gender were converted into 
numerical values. 
• The dataset was split into: 
o 80% training data 
o 20% testing data 
4. Model Training 
Two SVM models were trained using the prepared dataset: 
• Linear Kernel SVM 
• Polynomial Kernel SVM 
5. Model Evaluation 
To evaluate the models, we used the F1-score, which measures how well the model 
correctly predicts both classes. 
6. Probability Distribution Visualization 
We also created histogram plots of predicted probabilities for both classes: 
• Customers who stayed 
• Customers who exited 
Key Takeaways 
• Machine learning models can help identify customers who may leave the bank. 
• Feature preparation and scaling are important steps for improving model 
performance. 
• Using different SVM kernels allows the model to capture different types of 
relationships in the data. 
• The Polynomial Kernel SVM performed better for this dataset. 
Conclusion 
In this project, two Support Vector Machine models were trained to predict customer 
churn. 
The Polynomial Kernel SVM achieved the better performance, indicating that the 
customer data contains more complex relationships. 
With further improvements and additional features, this type of model could help banks 
identify customers at risk of leaving and take actions to retain them. 
