import pandas as pd
import numpy as np
data=pd.read_csv(r'C:\Users\Student\Downloads\DS.csv')

list=[data.head(1)]
print(list)

newData=data
for i,j in data.iterrows():
 if(j.Goes=="No"):
   continue
 else:
        if(j.Time==data.iloc[[i+1],[j.Time]]):
            print("Hello")
