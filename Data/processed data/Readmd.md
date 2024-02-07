To process the data, use this piece of code:
```python
from sklearn.preprocessing import StandardScaler

print("原始数据:")
df.head()  # 假设这里显示DataFrame的前几行作为示例

# 去掉'sex'变量
scaler = StandardScaler()
X_scaled = scaler.fit_transform(df.drop(['sex'], axis=1))

print("标准化后数据:")
X_scaled[:5]  # 显示标准化后数据的前五行作为示例
```
