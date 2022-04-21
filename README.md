answer 1
python code 
import pandas as pd
import numpy as np
df=pd.read_csv("main.csv")
mean_value=df['price'].mean()
df['price'].fillna(value=mean_value, inplace=True)
df.to_csv('answer.csv')
