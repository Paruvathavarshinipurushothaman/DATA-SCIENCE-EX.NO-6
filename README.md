# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("titanic_dataset.csv")
 df.head()
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```
<img width="985" height="431" alt="image" src="https://github.com/user-attachments/assets/238606e6-94bc-418c-829b-2acd833d23a9" />
<img width="588" height="478" alt="image" src="https://github.com/user-attachments/assets/d817d3cb-4393-4c7e-b591-b6fff5651642" />
<img width="602" height="481" alt="image" src="https://github.com/user-attachments/assets/0810c710-785c-4185-aa9e-c965b271aa3e" />
<img width="759" height="520" alt="image" src="https://github.com/user-attachments/assets/fd6fd382-4f22-4919-b6f8-cd16e2f1009c" />
<img width="649" height="505" alt="image" src="https://github.com/user-attachments/assets/a8196078-111b-4f5e-8d2e-cd8e9bd69a6c" />
<img width="643" height="504" alt="image" src="https://github.com/user-attachments/assets/0af73030-258f-43d0-ac80-1efbd5a4f0f1" />
<img width="645" height="495" alt="image" src="https://github.com/user-attachments/assets/f35b647a-ff69-4201-b0e3-f950aff1ed61" />
<img width="625" height="502" alt="image" src="https://github.com/user-attachments/assets/5d2552e8-71c6-4d95-8f12-952db53433ae" />
<img width="654" height="517" alt="image" src="https://github.com/user-attachments/assets/46b614fb-50f0-41d6-a461-303c4e60928b" />
<img width="649" height="494" alt="image" src="https://github.com/user-attachments/assets/950f2174-e1f3-4296-943c-9ad6e8f9d786" />
<img width="646" height="555" alt="image" src="https://github.com/user-attachments/assets/81cf09e4-ed66-4342-8691-e89c2ab41df9" />

## Result:
Thus, the Data Visualization using seaborn python library for the given data is implemented successfully.



