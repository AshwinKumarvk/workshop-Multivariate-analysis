# workshop-Multivariate-analysis

# AIM

To perform Multivariate EDA on the given data set.

Explanation Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.

# Algorithm

Step1

Import the built libraries required to perform EDA and outlier removal.

Step2

Read the given csv file.

Step3

Convert the file into a dataframe and get information of the data.

Step4

Return the objects containing counts of unique values using (value_counts()).

Step5

Plot the counts in the form of Histogram or Bar Graph.

Step6

Use seaborn the bar graph comparison of data can be viewed.

Step7

Find the pairwise correlation of all columns in the dataframe.corr()

Step8

Save the final data set into the file.

# Types of bivariate analyis

1)Numerical & Numerical(Scatter plot) 2)Numerical & Categorical(Bar plot,Box plot,Dist plot)

# Code

import pandas as pd

import numpy as py

import seaborn as sns

import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])

df

df.head()

df.info()

df.describe()

df.isnull().sum()

df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])

sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)

df.corr()

# Output

Data Head

![image](https://user-images.githubusercontent.com/95520655/229690989-cf917060-4af5-44a2-9add-a98b35fefe85.png)

Data Information

![image](https://user-images.githubusercontent.com/95520655/229691300-863e50c1-73bd-47d1-8b65-9ba94520253e.png)

Numerical & Numerical(Scatter plot)

![image](https://user-images.githubusercontent.com/95520655/229691640-cb189acd-c610-4081-bf20-a6959c75efd8.png)

Numerical & Categorical(Bar plot)

![image](https://user-images.githubusercontent.com/95520655/229691694-588d64a7-67bc-4b22-aede-ca86a74d516f.png)

Non-Graphical method(correlation)

![image](https://user-images.githubusercontent.com/95520655/229691776-2a6741b8-e2a3-42e6-8777-db2fb3d68b8c.png)

# Result

Thus we have performed Multivariate EDA on the given data set.
