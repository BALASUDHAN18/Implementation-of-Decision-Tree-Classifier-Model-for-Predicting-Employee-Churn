# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.

2.Read the data set.

3.Apply label encoder to the non-numerical column inoreder to convert into numerical values.

4.Determine training and test data set.

5.Apply decision tree Classifier and get the values of accuracy and data prediction. 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: BALASUDHAN P
RegisterNumber: 212222240017

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
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
```

## Output:

![240549984-db555cf9-2e00-410b-ad15-75b6c1613d53](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/ea2c5d9c-5c31-49aa-bc6a-58138e2c6c76)

![240550039-5f8554c1-f2ee-45b6-8884-13df04e1685d](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/42bdbbeb-1bb4-4fff-b4e3-6d2557bda718)

![240550097-34734c62-c365-4ad9-a4ec-39c6ec2c2189](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/06e493a8-e100-48aa-8b00-01b5bc54af48)

![240550188-36085f9f-3313-4c98-b9d4-31e17db70216](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/7ff59bdf-dc50-460f-93fe-3dcc04d170ca)

![240550264-4618ff86-838c-4ab1-b6c0-90ef1e446208](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/ba2d77f3-c5e2-48e3-bb9c-3bf77688d5fd)


![240550321-477141e1-1dd8-470c-becb-36580e52902c](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/702d9216-f2cb-4378-bffa-0853c1672bc1)

![240550386-55fba8ce-a272-41d0-a6fe-075c36f8c7b6](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118807740/6bac730e-0a7d-40cb-a49f-17c341deee0f)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
