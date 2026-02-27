# Task-1-Data-immersion-Wrangling-phase
import pandas as pd
 df= pd.read_excel("/Data_Immersion_Wrangling_Dataset_15000.xlsx")
print(df.head())
print(df.info())
df.columns
df.shape              
df.duplicated().sum() 
df.isnull().sum()     
df.describe() 
df['Order_Date'] = pd.to_datetime(df['Order_Date'])
df['Shipping_Date'] = pd.to_datetime(df['Shipping_Date'])
df['Date_of_Birth'] = pd.to_datetime(df['Date_of_Birth'])
df.info()
