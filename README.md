# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score

## Program:
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: PRIYANKA S
RegisterNumber:  212222040125

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()    #no departments and no left
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])

*/

## Output:
![243092961-28a02272-d076-488b-bc0e-258db61a3b29](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/a3d66a8f-75bf-48fc-a91a-2135670020c2)

![243092973-cdc55078-656b-49d7-b171-ba2be9a56bfd](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/f8a333ba-bb33-4c5c-8dec-368f28ffb186)

![243092986-c8005750-fb30-47db-9c4d-6309e48560b7](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/a62dafc1-4f72-4d27-ad87-ad853cfdaa24)

![243093015-8cbea8e5-088d-4896-8c3f-eabcedd9b7a0](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/d6440e76-21f8-40cc-8776-0f17cef52da7)

![243093033-7123868e-1b73-448a-a92c-bfcb52c69d22](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/156d0d19-df2b-4aa4-9512-194e29daee78)

![243093038-7900550f-09ae-4b93-baa2-4e1d8cd21967](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/384afecc-4bc1-44fb-bf6f-dff74b93aa92)

![243093038-7900550f-09ae-4b93-baa2-4e1d8cd21967](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/1e39f738-a9d1-49bc-8e7b-9ee9dcde25ed)

![243093071-d6235dee-d231-4eb2-9540-5a8fcc8d845f](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/e8cd47e8-ceaa-449f-8bde-c45edbac30eb)

![243093083-79384c60-837a-474e-adc4-cb88724287ce](https://github.com/PriyaThilagam/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119393798/0356f009-69f1-4c6b-a108-c588c9072daa)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
