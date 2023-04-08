# Ex03-Univariate-Analysis
## Aim:

To read the given data and perform the univariate analysis with different types of plots.

## Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm:

## Step1:
Read the given data.

## Step2:
Get the information about the data.

## Step3:
Remove the null values from the data.

## Step4:
Mention the datatypes from the data.

## Step5:
Count the values from the data.

## .Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.
## program
import pandas as pd 
import numpy as np 
df=pd.read_csv("/content/SuperStore (1).csv")
df.head()
![image](https://user-images.githubusercontent.com/86044259/192247626-9881035e-de6b-4cbe-a285-57040540c6fe.png)


df.isnull().sum()
![image](https://user-images.githubusercontent.com/86044259/192247711-ff09b84d-f052-4f70-9a59-765aa59ccf83.png)


df.info()
![image](https://user-images.githubusercontent.com/86044259/192247835-72a3f1c5-f519-4c0e-8b48-8926b6c0069a.png)


df.dtypes
![image](https://user-images.githubusercontent.com/86044259/192247987-7d0f59ad-2777-473a-8cc1-b0a273862ff0.png)


df.dtypes
![image](https://user-images.githubusercontent.com/86044259/192248060-4720a795-c1dd-4204-9aeb-b6b9215b6474.png)


import pandas as pd
import seaborn as sns
sns.boxplot(x='Sales',data=df)
![image](https://user-images.githubusercontent.com/86044259/192248153-1cdcbacf-3138-48f0-90ca-7e1fb83d1ff9.png)


import pandas as pd
import seaborn as sns
sns.countplot(x='Postal Code',data=df)
![image](https://user-images.githubusercontent.com/86044259/192248243-209c36e7-9f95-4fff-b5ab-5155039d887c.png)


import pandas as pd
import seaborn as sns
sns.displot(df["Postal Code"])
![image](https://user-images.githubusercontent.com/86044259/192248537-edab457b-ea61-4ceb-a394-d9ad181d7cc0.png)


import pandas as pd
import seaborn as sns
sns.histplot(x="Postal Code",data=df)
![image](https://user-images.githubusercontent.com/86044259/192248619-6b1c05fd-9c55-440e-82bf-bf0c754e5e3f.png)


import pandas as pd
import seaborn as sns
df=pd.read_csv("/content/SuperStore (1).csv")
df.skew()
![image](https://user-images.githubusercontent.com/86044259/192248984-f9bbb521-4670-4389-b78a-29916ad05c00.png)


import pandas as pd
import seaborn as sns
sns.histplot(x='Sales',data=df)
![image](https://user-images.githubusercontent.com/86044259/192249061-9f8e62db-db36-4ea9-912f-6820dbc1ade2.png)



import pandas as pd
import seaborn as sns
sns.displot(x='Sales',data=df)
![image](https://user-images.githubusercontent.com/86044259/192249169-959a00c3-43f7-43d4-8c2f-c36d637b4138.png)
## Result:

Thus we have read the given data and performed the univariate analysis with different types of plots.
