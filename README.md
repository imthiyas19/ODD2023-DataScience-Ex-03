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

## Diabetes.csv:



![273362610-419e9958-ebfc-4655-a1a8-2c454cb74850](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/ccc49495-ec37-46ff-9fca-f23e542c2961)


![273362614-f9f618de-821f-4f83-8a3c-39ec10b2daa1](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/744c6e3e-37a7-47d0-aca2-398d5a721422)


![273362620-ec99b681-0d52-44fc-9856-8497f1b364f1](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/e210d56a-3792-4d2f-91a8-6cc15b31dd89)


![273362622-faeeeb7f-8c98-4aac-831d-4290b13a37af](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/7d3ddb09-234d-4aab-a98b-6d4c1fd10560)

![273362627-f057cb51-05ad-4be5-8f47-ade851937a7b](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/cec847b6-0f8d-4287-b83e-8c682dd72b7e)



![273362631-92ac30ae-0008-4782-a978-51a18375c6cf](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/146a8f97-9fed-4d5c-ade5-8d790e2184bb)

![273362637-8d94b215-755f-4463-b31a-3e621c6c9737](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/b643a9a6-a360-4298-8e98-38f4287bb6b4)


![273362646-149d2c19-839e-4036-9fcf-3a1504b31d9f](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/fc1a37f2-a2be-479d-ab5e-51f3f611eabd)




![273362650-78a8a86f-59d3-478c-a43f-824bfef018b5](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/1a2a1329-af74-4d78-b036-6983529354b1)



![273362652-d81a742e-ac55-4f8e-94b6-1d6756337d4f](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/2edba393-f716-466c-81b7-6a4b57246c65)

## employeesal.csv:



![273362676-62ea18d6-80fe-4226-a2bf-e8ac7b7be70f](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/169dce7e-48fd-498e-a9dc-10b0f9d11170)





![273362684-22ff195d-7803-4bb8-b327-75d552c0bc11](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/22a8cba2-a8ac-4c3f-adc9-a86e45f8bfba)




![273362694-adbf097c-c021-4022-908f-c3560d4ef3d8](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/f6a825a8-eb7c-4e9f-9403-f0c02f719303)



![273362696-69709fbf-cb55-479c-9c2c-72998f2534da](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/07b387cc-fec2-4c56-b67c-21accc6a5fac)



![273362698-622006e5-1c9d-4476-8b79-6d25cc3038c6](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/42d865ab-3ddc-4dac-9f92-aeec84c621e4)




![273362702-02b56aec-5b8f-4b85-b109-62fe7b327140](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/8376bfdb-1741-4f4b-a2e0-b6bfbd9d47cc)




![273362705-a05cd1a9-cbac-412c-879f-696686b088d4](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/1c759bd9-bcfd-45f1-a5fc-a974ba0e9530)


![273362730-95f17453-ae0b-4a2f-8630-06c03517c0f9](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/9e0dc11a-9c31-4be9-90b1-34293738cdb3)


![273362720-f4fe5542-468a-42b5-b0bb-9a1eef28d63f](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/73933f7d-e142-4308-9324-ec13e236385c)



![273362716-57d88365-43f0-4a7a-a0b7-276cb5af4c44](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/49f953da-ef0c-4708-a689-6f4eb82b9d5c)



![273362711-57275b31-53fa-4f65-aa89-3daa20daa89d](https://github.com/imthiyas19/ODD2023-DataScience-Ex-03/assets/120353416/90e8ed33-77b2-4b22-9962-2dbecd0c9e89)

# RESULT:

Hence the univariate analysis is verified
































