# ODD2023-DataScience-Ex-03
# Aim:
To read the given data and perform the univariate analysis with different types of plots.

Explanation: Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
Step1 Read the given data.

Step2 Get the information about the data.

Step3 Remove the null values from the data.

Step4 Mention the datatypes from the data.

Step5 Count the values from the data.

###  Program:
```
Developed By : MOHAMMED IMTHIYAS.M
Register number: 212222230083
```
# Superstore.csv:
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
### Diabetes.csv:
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
### employeesal.csv:
```
import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
### Output:
## Superstore.csv:




![273362524-281a0659-c9b2-4d95-91de-33540c853bd1](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/f68f6abb-d614-4ac2-87b3-71db4d43e2b8)



![273362534-42f6da91-760a-489d-99c4-758785f5467c](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/64aefaf8-8202-41cc-93d6-e9402089992c)

![273362536-274d5f69-0e5a-49af-a6e5-54c627e81234](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/aa8e2098-0abd-4308-b7c6-faf39a4d21dc)






![273362543-418809b8-1921-435a-8614-6170a8235472](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/31d9a8b4-36d9-4d5c-ad04-1289978c2e0d)


![273362557-418a705e-613d-4db7-ab00-e0eea0c8015d](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/a2c95e20-55bc-4727-b60b-d33a55694b0c)



![273362562-df21227b-a33d-400a-adde-ab13c891247e](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/c2b52cad-71b6-4989-98e3-f88f847a109c)


![273362576-57ee4d74-0ce9-4993-a9b5-efeb75a8eb73](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/ff467f26-05e6-4474-a931-4865de097d13)

![273362581-1cd58b20-e7a4-4f9d-b148-8309b23901b5](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/f23ea6e1-46f9-4308-a73f-65f022f46c05)



![273362585-7c8d28e5-4aa4-4f08-aa8f-701451dcf0d2](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/b1f8537e-7a25-49bc-9685-3eb927551972)

























