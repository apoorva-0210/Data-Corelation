# Data-Corelation
#To find out the correlation of data

import pandas as pd
import numpy as np
import seaborn as sns

data=pd.read_csv('My_data.csv')

#For tabular correlation
data.corr()

#For heatmap correlation with values
plt.figure(figsize=(15,8)) 
sns.heatmap(data.corr(), annot=True, cmap="Blues")
