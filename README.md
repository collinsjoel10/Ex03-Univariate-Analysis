# Ex03-Univariate-Analysis
Aim:

To read the given data and perform the univariate analysis with different types of plots.

Explanation:

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

Algorithm:

Step1:
Read the given data.

Step2:
Get the information about the data.

Step3:
Remove the null values from the data.

Step4:
Mention the datatypes from the data.

Step5:
Count the values from the data.

Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.

Program:

SuperStore.csv

```
import pandas as pd 
import numpy as np 
import seaborn as sns
df=pd.read_csv('superstore.csv') df
df.head() df.info() df.describe() df.isnull().sum()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```

OUTPUT

![Screenshot (54)](https://user-images.githubusercontent.com/118626456/228298437-6614c4f0-e445-4346-b40c-cdff3ad6ceb7.png)
![Screenshot (55)](https://user-images.githubusercontent.com/118626456/228298484-4f27ebdd-73d9-43a1-8571-431b4805353d.png)
![Screenshot (56)](https://user-images.githubusercontent.com/118626456/228298525-187d1a86-3f12-43fd-9891-a24934794f37.png)
![Screenshot (57)](https://user-images.githubusercontent.com/118626456/228298583-5e28f857-03ed-476b-84d9-e409f2825bca.png)
![Screenshot (58)](https://user-images.githubusercontent.com/118626456/228298608-650fd7de-28a2-4f9c-919e-5debda4c5045.png)
![Screenshot (59)](https://user-images.githubusercontent.com/118626456/228298628-1d0b59fb-5a3b-489b-86fb-28239d9783c0.png)
![Screenshot (60)](https://user-images.githubusercontent.com/118626456/228298658-e12b601c-722a-4814-955e-31250db087bf.png)
![Screenshot (61)](https://user-images.githubusercontent.com/118626456/228298797-f0c9a754-7168-4e0d-bcb2-be1f3592f651.png)
![Screenshot (62)](https://user-images.githubusercontent.com/118626456/228298840-6f90af4a-8dbe-4e32-923c-b753979d364e.png)
![Screenshot (63)](https://user-images.githubusercontent.com/118626456/228298863-176688b4-eb7a-4717-ba47-bef2d2fe54fd.png)
![Screenshot 2023-03-28 114943](https://user-images.githubusercontent.com/118626456/228298894-97b0eefb-d2e7-42b5-bb2c-5c4fe7cee5b6.png)

RESULT

Thus we have read the given data and performed the univariate analysis with different types of plots.











