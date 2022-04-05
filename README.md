# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file


# CODE
import pandas as pd
df = pd.read_csv("Data_set.csv")
df.head(10)
df.tail()
df.info()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df.head(10)
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df.head()
df['rating']=df['rating'].fillna(df['rating'].mean())
df.info()
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df.info()
df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])
df.info()
[df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mode()[0])
df.info()
df['watchers']=df['watchers'].fillna(df['watchers'].mode()[0])
df.head()
df.info()
df.isnull().sum()
# OUPUT
![WhatsApp Image 2022-04-05 at 9 17 15 AM](https://user-images.githubusercontent.com/103016377/161678493-8c8568a3-af9d-4afe-a29b-00b70c80b96b.jpeg)
![WhatsApp Image 2022-04-05 at 9 17 15 AM (5)](https://user-images.githubusercontent.com/103016377/161678514-8e1dcebc-b5bf-4a7e-b4ae-748aa4844376.jpeg)
![WhatsApp Image 2022-04-05 at 9 17 15 AM (4)](https://user-images.githubusercontent.com/103016377/161678520-bed5ff99-a8cc-4ab3-ad45-dfd39e22d8a1.jpeg)
![WhatsApp Image 2022-04-05 at 9 17 15 AM (3)](https://user-images.githubusercontent.com/103016377/161678523-53a9834d-e4e2-428f-a6b1-01cb4486ef24.jpeg)
![WhatsApp Image 2022-04-05 at 9 17 15 AM (2)](https://user-images.githubusercontent.com/103016377/161678524-ad440041-9988-4cf0-8268-799017c8c750.jpeg)
![WhatsApp Image 2022-04-05 at 9 17 15 AM (1)](https://user-images.githubusercontent.com/103016377/161678526-d3f5c8a1-6c83-4ab9-9e22-b47abe7eb489.jpeg)

