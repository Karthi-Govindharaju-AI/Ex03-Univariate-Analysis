# Ex03-Univariate-Analysis
## Aim
To read the given data and perform the univariate analysis with different types of plots.

## Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm
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
```
Developed By :VIGNESH R
reference number: 21222230172
```
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

![Screenshot 2023-03-27 203824](https://user-images.githubusercontent.com/118680410/228207821-4c5919f1-2ef7-4c93-89fe-10e0d11c530a.png)
![Screenshot 2023-03-28 155312](https://user-images.githubusercontent.com/118680410/228207826-a8c4eede-6fc5-4fbf-b7ec-23f1b49917b7.png)
![Screenshot 2023-03-28 155321](https://user-images.githubusercontent.com/118680410/228207836-624685a0-434e-4d37-9204-ed2351b96b07.png)
![Screenshot 2023-03-28 155331](https://user-images.githubusercontent.com/118680410/228207841-16c5791c-9fa3-4e75-9a82-3688e6cd80c8.png)
![Screenshot 2023-03-28 155339](https://user-images.githubusercontent.com/118680410/228207844-26a4e0ee-4b72-4ae7-86aa-b3498290fc69.png)
![Screenshot 2023-03-28 155346](https://user-images.githubusercontent.com/118680410/228207850-78aa3991-ecbc-407d-9fff-a663ffa780f6.png)
![Screenshot 2023-03-28 155353](https://user-images.githubusercontent.com/118680410/228207853-f70cc0bb-b67a-4e4f-a770-b4e23ce064ab.png)
![Screenshot 2023-03-28 155400](https://user-images.githubusercontent.com/118680410/228207859-9db566f0-268b-4e82-a056-1b7466ddead5.png)
![Screenshot 2023-03-28 155412](https://user-images.githubusercontent.com/118680410/228207862-c616fd40-ea50-4ccc-82ff-6ae1c394be55.png)

## Diabetes.csv

![Screenshot 2023-03-30 211938](https://user-images.githubusercontent.com/118680410/228897098-9b03b1fb-2e9e-4a5c-8629-f1321503f78c.png)
![Screenshot 2023-03-30 211953](https://user-images.githubusercontent.com/118680410/228897290-c32a6b68-99c7-464c-adf1-c943222bab52.png)

![Screenshot 2023-03-30 212008](https://user-images.githubusercontent.com/118680410/228897321-3afa4c14-bac9-460c-86eb-4b569f1140fb.png)
![Screenshot 2023-03-30 212024](https://user-images.githubusercontent.com/118680410/228897343-9b533df9-5808-41ba-b926-a6c368a560b7.png)
![Screenshot 2023-03-30 212037](https://user-images.githubusercontent.com/118680410/228897356-1d8ad723-96f1-4ca2-9abb-dabb003bc0a3.png)
![Screenshot 2023-03-30 212047](https://user-images.githubusercontent.com/118680410/228897410-eb383e4d-6785-45d9-8ab3-3721edde23bd.png)
![Screenshot 2023-03-30 212101](https://user-images.githubusercontent.com/118680410/228897476-8d958b34-2f05-44cf-9eb7-14cec6e69b3a.png)
![Screenshot 2023-03-30 212111](https://user-images.githubusercontent.com/118680410/228897549-056925e3-9be1-4e64-8b9d-a6063c5da099.png)
![Screenshot 2023-03-30 212127](https://user-images.githubusercontent.com/118680410/228897590-b123a0d1-93de-457a-8bf7-0e92f1f24cdd.png)
![Screenshot 2023-03-30 212137](https://user-images.githubusercontent.com/118680410/228897642-560def56-cb8e-4359-bad2-1e2f03d159ed.png)
# RESULT
Hence the univariate analysis is verified
