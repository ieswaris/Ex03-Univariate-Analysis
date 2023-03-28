## Ex03-Univariate-Analysis

# Aim
To read the given data and perform the univariate analysis with different types of plots.

# Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm
Step1
Read the given data.

Step2
Get the information about the data.

Step3
Remove the null values from the data.

Step4
Mention the datatypes from the data.

Step5
Count the values from the data.

Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

# Program
Developed by :ESWARI S

Registration Number : 212221220012

import pandas as pd

import numpy as np

import seaborn as sns

df=pd.read_csv('superstore.csv')

df

df.head()

df.info()

df.describe()

df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)

sns.countplot(x='Postal Code',data=df)

sns.distplot(df["Postal Code"])

sns.histplot(x='Postal Code',data=df)

# Output
## DATA

![image](https://user-images.githubusercontent.com/127847210/228205834-ab760153-1939-4282-acd7-376749ae02bd.png)



## DATA HEAD

![image](https://user-images.githubusercontent.com/127847210/228206164-339272c2-bafa-4207-9061-171de7b709b9.png)



## DATA INFORMATION

![image](https://user-images.githubusercontent.com/127847210/228206651-f0799582-b2ab-4264-8625-3ed7796049be.png)


## DATA DESCRIBE

![image](https://user-images.githubusercontent.com/127847210/228206919-2b64e959-aae7-4886-a487-63986887e911.png)


## DATA NULL VALUES

![image](https://user-images.githubusercontent.com/127847210/228207691-87c910d2-dfc2-4c74-92ce-df5db195daee.png)


## DATA'S DATATYPES

![image](https://user-images.githubusercontent.com/127847210/228207869-f95d8253-c6ea-4262-8e68-50a2036ac5f6.png)


## DATA'S VALUECOUNT

![image](https://user-images.githubusercontent.com/127847210/228208046-483d441e-b993-4745-9b66-4eccb7e3306b.png)


## BOXPLOT

![image](https://user-images.githubusercontent.com/127847210/228208141-14756946-f76b-4ece-bc33-f6039af68b3e.png)


## COUNTPLOT

![image](https://user-images.githubusercontent.com/127847210/228208211-f7a6f04d-6629-4366-bf62-e8cf3fad6d52.png)


## DISTRIBUTION PLOT

![image](https://user-images.githubusercontent.com/127847210/228208289-7a9141bc-ac72-490d-876c-fc54c0a4bc1f.png)


## HISTOGRAM PLOT

![image](https://user-images.githubusercontent.com/127847210/228208389-7ff59c53-2ff0-49bc-a7d0-ce79a2de369e.png)


# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.



