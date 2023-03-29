
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



# Output:
![](/1.png)
![](/2.png)
![](/3.png)
![](/4.png)
![](/5.png)
![](/6.png)
![](/7.png)
![](/8.png)
![](/9.png)
![](/10.png)
![](/11.png)
![](/12.png)
![](/13.png)
![](/14.png)
![](/15.png)
![](/16.png)

# Result:
Thus we have read the given data and performed the univariate analysis with different types of plots.
