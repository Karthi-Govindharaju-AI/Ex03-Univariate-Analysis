# Ex03-Univariate-Analysis
## Aim
To read the given data and perform the univariate analysis with different types of plots.

## Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Step1
Read the given data.

## Step2
Get the information about the data.

## Step3
Remove the null values from the data.

## Step4
Mention the datatypes from the data.

## Step5
Count the values from the data.
superstore.csv
Developed By : NIKHIL M
reference number: 212222230095
## Superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```

## Diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
# OUTPUT
## Superstore.csv
Screenshot 2023-03-27 203824 Screenshot 2023-03-28 155312 Screenshot 2023-03-28 155321 Screenshot 2023-03-28 155331 Screenshot 2023-03-28 155339 Screenshot 2023-03-28 155346 Screenshot 2023-03-28 155353 Screenshot 2023-03-28 155400 Screenshot 2023-03-28 155412

# OUTPUT 
## Diabetes.csv
Screenshot 2023-03-30 211938 Screenshot 2023-03-30 211953

Screenshot 2023-03-30 212008 Screenshot 2023-03-30 212024 Screenshot 2023-03-30 212037 Screenshot 2023-03-30 212047 Screenshot 2023-03-30 212101 Screenshot 2023-03-30 212111 Screenshot 2023-03-30 212127 Screenshot 2023-03-30 212137
# RESULT
Hence the univariate analysis is verified
