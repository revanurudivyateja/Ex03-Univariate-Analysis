import pandas as pd
import numpy as np
import seaborn as snb
df = pd.read_csv('/content/SuperStore.csv')
df.head(10)
df.info()
df.describe()
df.dtypes
df.isnull().sum()
df['Postal Code'] = df["Postal Code"].fillna(df['Postal Code'].mode()[0])
df.isnull().sum()
df['Postal Code'].value_counts()
snb.boxplot(x="Sales",data=df)
snb.countplot(x="Sales",data=df)
snb.distplot(df["Sales"])
snb.histplot(x="Sales",data=df)
df.skew()
df.kurtosis()
snb.histplot(x="Postal Code",data=df)
snb.displot(x="Postal Code",data=df)
snb.boxplot(x="Postal Code",data=df)
snb.boxplot(x="Row ID",data=df)
snb.histplot(x="Ship Mode",data=df)
snb.countplot(x="Category",data=df)
*/
