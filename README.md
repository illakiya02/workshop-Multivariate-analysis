# workshop-Multivariate-analysis
import pandas as pd
import seaborn as sns
excel_file='/content/FlightInformation.xlsx'
df=pd.read_excel(excel_file)
print(df)
![image](https://user-images.githubusercontent.com/112244898/230832162-3bd071ec-537c-452d-883e-f12adf52a569.png)
df.dtypes
![image](https://user-images.githubusercontent.com/112244898/230832241-29d2a00f-bc14-4bd6-8d1c-0d48bec61b08.png)
sns.scatterplot(y=df['Price'],x=df['Total_Stops'],data=df)
![image](https://user-images.githubusercontent.com/112244898/230832318-e5d21589-51c7-43e1-bb59-62ae79571452.png)
sns.barplot(y=df['Price'],x=df['Source'],data=df)
![image](https://user-images.githubusercontent.com/112244898/230832399-62fcced4-7944-4e03-a2dc-399c479a1240.png)
df.info()
![image](https://user-images.githubusercontent.com/112244898/230832469-c1c06ee7-2497-4005-ab60-7a3246d4e667.png)
df.corr()
![image](https://user-images.githubusercontent.com/112244898/230832588-51c158f7-87c8-4f51-a5e4-b58e114cb79c.png)
sns.heatmap(df.corr(),annot=True)
![image](https://user-images.githubusercontent.com/112244898/230832665-4233d39b-ca9c-4e05-8585-71db44194276.png)

