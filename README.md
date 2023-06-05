# Exp-10


## AIM
To Perform Data Visualization on a complex dataset and save the data to a file

## EXPLANATION

Data visualization is the graphical representation of information and
data. By using visual elements like charts, graphs, and maps, data visualization tools
provide an accessible way to see and understand trends, outliers, and patterns in
data.

## ALGORITHM

STEP 1
Read the given Data

STEP 2
Clean the Data Set using Data Cleaning Process

STEP 3
Apply Feature generation and selection techniques to all the features of the data set

STEP 4
Apply data visualization techniques to identify the patterns of the data.

## CODE
/*
**Data Visualization - Iris.csv**

import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

df = pd.read_csv("/content/iris.csv")

df.head()

df.info()

df["variety"].value_counts()

sns.countplot(x='variety', data=df, )

plt.show()

sns.scatterplot(x='sepal.length', y='sepal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.scatterplot(x='petal.length', y='petal.width', hue='variety', data=df, )

plt.legend(bbox_to_anchor=(1, 1), loc=2)

plt.show()

sns.pairplot(df.drop(['Id'], axis = 1), hue='variety', height=2)

fig, axes = plt.subplots(2, 2, figsize=(10,10)) 

axes[0,0].set_title("Sepal Length")

axes[0,0].hist(df['sepal.length'], bins=7) 

axes[0,1].set_title("Sepal Width")

axes[0,1].hist(df['sepal.width'], bins=5); 

axes[1,0].set_title("Petal Length")

axes[1,0].hist(df['petal.length'], bins=6); 

axes[1,1].set_title("Petal Width")

axes[1,1].hist(df['petal.width'], bins=6);

sns.heatmap(df.corr(method='pearson').drop(['Id'], axis=1).drop(['Id'], axis=0), annot = True);

plt.show()


## OUTPUT 

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/2c0e861c-e912-4664-ac84-82612b49d6ae)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/68043b70-ff88-4d26-9b19-95b20d62bfe7)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/c948f4e5-ea91-4e74-9b3a-94b4d8550178)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/cd21a8ff-2f41-4bd3-99a0-2b62c801c4c0)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/56445ee3-d0f8-482e-8630-b44b8be09bca)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/9ad3772b-44cf-4f60-9b1e-d02d4ed04383)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/5be1c119-e7ac-4ed6-9d14-811100847c05)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/aa3c0624-043f-43e4-b924-ae1e3293a357)

![image](https://github.com/AshwinKumarvk/Ex-10-DS/assets/95520655/d9500540-208f-4533-b719-21bfbe44a4a5)




## RESULT

Thus the Data Visualization for the given dataset had been executed successfully. 
