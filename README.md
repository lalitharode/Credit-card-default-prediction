# Credit-card-default-prediction
Analyzing the credit card database to find default/non default

# Credit-Card-Default-Prediction---Capstone-Project

![772971-credit-card-shutterstock](https://user-images.githubusercontent.com/103633582/183985508-a2f3e92c-ff73-448b-a108-6140180bef8e.jpg)



-----------------------------------------------------

# 📋 Introduction -

Credit cards are usually small plastic cards with a unique number attached to an account.
Credit cards impose the condition that cardholders pay back the borrowed money, plus any applicable interest, as well as any additional agreed-upon charges, either in full by the billing date or over time.


-----------------------------------------------------

# 📋 Dataset - 

We used the [Credit Card Default payment in Taiwan]  to predict whether the credit card holders are defaulters or Non-defaulters. The Dataset and its attributes are described below

ID: ID of each client

LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit

SEX: Gender (1=male, 2=female)

EDUCATION: (1= post graduate , 2=graduate, 3=higher secondary , 4=others, 5=unknown, 6=unknown)

MARRIAGE: Marital status (1=married, 2=unmarried, 3=others)

AGE: Age in years

PAY_0: Repayment status in April (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months,8=payment delay for eight months, 9=payment delay for nine months and above)

PAY_2: Repayment status in may,  (scale same as above)

PAY_3: Repayment status in june (scale same as above)

PAY_4: Repayment status in july  (scale same as above)

PAY_5: Repayment status in August  (scale same as above)

PAY_6: Repayment status in september  (scale same as above)

BILL_AMT1: Amount of bill statement in April (NT dollar)

BILL_AMT2: Amount of bill statement in May (NT dollar)

BILL_AMT3: Amount of bill statement in June (NT dollar)

BILL_AMT4: Amount of bill statement in july (NT dollar)

BILL_AMT5: Amount of bill statement in August (NT dollar)

BILL_AMT6: Amount of bill statement in September (NT dollar)

PAY_AMT1: Amount of previous payment in April (NT dollar)

PAY_AMT2: Amount of previous payment in May (NT dollar)

PAY_AMT3: Amount of previous payment in june (NT dollar)

PAY_AMT4: Amount of previous payment in july (NT dollar)

PAY_AMT5: Amount of previous payment in August (NT dollar)

PAY_AMT6: Amount of previous payment in September (NT dollar)

default.payment.next.month: Default payment (1=yes, 0=no)

-------------------------------------

# 💾 Appraoch Method - 
Exploratory Data Analysis (EDA): In this part we have done some EDA on the features to see the trend.

## Data Processing:
In this part we applied SMOTE(Synthetic Minority Oversampling Technique) as the classes were unbalanced in the dataset. Also computed features based on feature importance.**pay_ARR_0 > pay_ARR_-1 > pay_ARR_-2 > pay_ARR_1 > Marriage married >Education Higher secondry** were the top features.

## Model Creation:
Finally in this part we created the various models. These various models are being analysed and we tried to study various models so as to get the best performing model for our project.

# 💾 Models Used - 

• Logistic Regression

• Decision Tree Classifier

• Random Forest Classifier

• K Nearest Neighbors

• Gradient Boosting

• XG Boosting

-----------------------------------------------------

# 💾 Conclusion -

In ML implementation i have used many algorithms like logistic regression, Decision tree, Random forest, KNN, Gradient boosting, XGboosting, among all them gradient boosting and XGboosting giving us a better result. but time taken for fitting by gradient boosting is more as compared to xgboosting, for final i will select a gradient boosting because,

1. *gradient boosting Classifier* has the best value of accuracy score of *87%*
2. *gradient boosting Classifier* has the best value of precision score of *81%*
3. *gradient boosting Classifier* has the best value of recall score of *92%*
4. *gradient boosting Classifier* has the best value of f1 score of *86%*
5. *gradient boosting Classifier* has the best value of Roc_auc score of *87%*

