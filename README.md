# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2. Upload the csv file and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: A.SANJAI
RegisterNumber: 212220040142 
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![image](https://user-images.githubusercontent.com/95969295/204552593-af7ef185-4e71-4203-9e0e-86710ccad863.png)

![image](https://user-images.githubusercontent.com/95969295/204552699-949481ec-7260-4090-9283-28b49d3c6d93.png)

![image](https://user-images.githubusercontent.com/95969295/204552826-b614f548-87ea-4fd8-a2fb-79c74b3399d9.png)

![image](https://user-images.githubusercontent.com/95969295/204552944-a637af64-11d3-4e07-87d6-f21ace194110.png)

![image](https://user-images.githubusercontent.com/95969295/204553038-278fd2e7-8075-4b8f-96de-5880c2992d32.png)

![image](https://user-images.githubusercontent.com/95969295/204553148-c8027273-ca3e-4a05-a812-0ecee8063951.png)

![image](https://user-images.githubusercontent.com/95969295/204553313-b662daf5-8a37-423c-9008-0aae2f14f0a9.png)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
