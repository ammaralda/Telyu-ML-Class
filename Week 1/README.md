House prediction using several model
- Linear Regression
- Decission Tree
- Random Forest

Preprocessing:
There are some columns that has missing value


![image](https://user-images.githubusercontent.com/57104367/156873007-eacd18fd-ed38-4317-8178-614b37c939c4.png)


And fill the missing value based on description

![image](https://user-images.githubusercontent.com/57104367/156873034-c50eaec3-b4c7-4ecc-abb0-adae326d0e63.png)

I add the missing value with mean and mode. There is one column that I change it into categorical since it has string as the mode.


Now we can plot the correlation as a heat map

![image](https://user-images.githubusercontent.com/57104367/156873193-129708f5-e65e-43d1-99c4-eda5bf10b1c7.png)

Next is, to change the categorical columns into numerical by using LabelEncoder provided by sklearn.

![image](https://user-images.githubusercontent.com/57104367/156873165-961d5e64-b47e-4e1d-971c-7fae6fd6b970.png)

Before we start train the model, we need to normalize all data so that it can trained properly.
Here, We are using MinMaxScaler to notmalize our dataset. Firstly, we need to import that class from sklearn.preprocessing package

![image](https://user-images.githubusercontent.com/57104367/156873231-151f2d2c-3db2-4b40-ac53-bd682e86e6ea.png)


Split dataset for train and test using 70% and 30% respectively.

![image](https://user-images.githubusercontent.com/57104367/156873271-cdcb611c-eb95-4827-85bc-f376cc64eff7.png)


Now we can start to train the dataset using each model




Scores:
![image](https://user-images.githubusercontent.com/57104367/156872842-be18d477-87e3-4a83-8a5c-f72681ee269d.png)


It is found that random forest has the highest accuracy and may provide more with hypertuning on its parameters



References


[1]W. Koehrsen, “Hyperparameter Tuning the Random Forest in Python,” Medium, Jan. 10, 2018. https://towardsdatascience.com/hyperparameter-tuning-the-random-forest-in-python-using-scikit-learn-28d2aa77dd74.
[2]V. Ukani, “Melbourne House Price Predic. Using ML-Model,” kaggle.com. https://www.kaggle.com/vikasukani/melbourne-house-price-predic-using-ml-model (accessed Mar. 05, 2022).
