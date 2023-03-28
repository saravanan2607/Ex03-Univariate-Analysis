## Ex03-Univariate-Analysis

# Aim:

To read the given data and perform the univariate analysis with different types of plots.

# Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

# Algorithm:

Step1:
Read the given data.

Step2:
Get the information about the data.

Step3:
Remove the null values from the data.

Step4:
Mention the datatypes from the data.

Step5:
Count the values from the data.A

Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.


# Program:
````
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
print(df)
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
sns.boxplot(x='Postal Code',data=df)
sns.countplot(x="Postal Code",data=df)
sns.histplot(x="Postal Code",data=df)
df.skew()
sns.histplot(x='Postal Code',data=df)
sns.displot(x="Postal Code",data=df)
df.kurtosis()
````

````
import pandas as pd
import seaborn as sns
df1=pd.read_csv("diabetes.csv")
print(df1)
df1.info()
df1.describe()
df.isnull().sum()
df1.dtypes
sns.boxplot(x='Glucose',data=df1)
sns.countplot(x="Glucose",data=df1)
sns.displot(df1["Glucose"]) 
sns.histplot(x="Glucose",data=df1)
df1.skew()
df1.kurtosis()
````


# Output:
## Dataset:

![dataset](https://user-images.githubusercontent.com/94165957/194359404-dbf8ccad-0d3b-43a2-8984-a18d694bac64.png)

## Head data:

![head](https://user-images.githubusercontent.com/94165957/194359364-46f68956-4de1-4361-8b4a-e284fa2c7665.png)

## Dataset Information:

![info](https://user-images.githubusercontent.com/94165957/194359292-8fc4ecaf-bc54-43f7-a50e-b722844f4ddd.png)

## Data Description:

![describe](https://user-images.githubusercontent.com/94165957/194359242-05df0748-5a96-4490-a4f1-b61e4f4dd079.png)


## Null data:

![null](https://user-images.githubusercontent.com/94165957/194359166-8a815c05-d2a2-4337-b8d5-e67196e829ee.png)

## Datatype:

![dtypes](https://user-images.githubusercontent.com/94165957/194359080-89ef8951-fdd3-46bd-b131-e32cf2ca63bd.png)


## Value counts:

![valuecounts](https://user-images.githubusercontent.com/94165957/194359000-c38df02d-59a2-410f-a86a-396cc93bc650.png)

## Box plot:
![boxplot](https://user-images.githubusercontent.com/94165957/194358960-b3fc93fa-cb6c-47bd-b9ea-2d330819053d.png)


## Count plot:

![countplot](https://user-images.githubusercontent.com/94165957/194358917-154fc777-a5ae-4d15-81a3-a8c6b56721cd.png)

## Distribution plot:

![distplot](https://user-images.githubusercontent.com/94165957/194358840-c0371f0a-3c88-4fc2-9ca3-2023abd425d4.png)

## Histogram plot:

![histplot](https://user-images.githubusercontent.com/94165957/194358822-1f99028a-a96f-403f-a8d0-5ac6ebdab265.png)

# Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.
