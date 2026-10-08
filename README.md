#find missing values
df.isnull().sum()
#in percentage
df.isnull().sum()/len(df)*100
#visulaization missing values
import seaborn as sns
sns.heatmap(df.isnull(),cbar=False,cmap='viridis')
