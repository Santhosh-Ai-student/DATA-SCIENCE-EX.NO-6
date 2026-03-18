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
import seaborn as sns
df=sns.load_dataset("tips")
df.head()

# Correlation Matrix
df.corr()
sns.heatmap(df.corr())

# Joint plot
# Univarate Analysis
sns.jointplot(x='tip',y='total_bill',data=df,kind='hex')
sns.jointplot(x='tip',y='total_bill',data=df,kind='reg')

# Pair Plot
sns.pairplot(df)
sns.pairplot(df,hue='sex')

# Dist Plot
sns.distplot(df['tip'])
sns.distplot(df['tip'],kde=False,bins=10)

## CATEGORICAL PLOTS
# Count plot
sns.countplot(y='sex',data=df)

# Bar plot
sns.barplot(x='sex',y='total_bill',data=df)
df.head()

# Box Plot
sns.boxplot(x="day", y="total_bill", data=df,palette='rainbow')

# Violin Plot
sns.violinplot(x="total_bill", y="day", data=df,palette='rainbow')
```
<img width="810" height="696" alt="image" src="https://github.com/user-attachments/assets/64f7cb25-49f9-42f0-8f9b-5c98cfcbc3fc" />
<img width="876" height="930" alt="image" src="https://github.com/user-attachments/assets/f708acb6-fa56-4a72-b7f7-d4b1fd178296" />
<img width="919" height="925" alt="image" src="https://github.com/user-attachments/assets/943f79ff-de28-47ae-b3f5-9efffe47d779" />
<img width="1047" height="924" alt="image" src="https://github.com/user-attachments/assets/c09a749f-bff5-4c15-a037-a1f0cde47214" />
<img width="1198" height="927" alt="image" src="https://github.com/user-attachments/assets/23e9bc40-199c-4ea5-b8ed-0de126d858c7" />
<img width="892" height="679" alt="image" src="https://github.com/user-attachments/assets/a8120863-c8a4-4cb0-89dd-91869b8d3c3c" />
<img width="902" height="716" alt="image" src="https://github.com/user-attachments/assets/ed0cc20e-289b-49b2-b5dc-7d8694fb3901" />

# Result:
Thus, performing Data Visualization using seaborn python library for the given datas has been executed successfully.
