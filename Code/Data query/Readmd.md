```python
# 导入所需库
from sklearn.preprocessing import StandardScaler
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.datasets import load_diabetes
import pandas as pd
import numpy as np

# 加载糖尿病数据集
diabetes = load_diabetes()
df = pd.DataFrame(data=np.c_[diabetes['data'], diabetes['target']],
                  columns=diabetes['feature_names'] + ['target'])

# 显示原始数据（这里仅显示部分，实际使用时请根据需要调整）
print("原始数据:")
# df.head()  # 示例：展示DataFrame的前五行

# 去掉'sex'变量并进行标准化处理
scaler = StandardScaler()
X_scaled = scaler.fit_transform(df.drop(['sex'], axis=1))
print("标准化后数据:")
# X_scaled[:5]  # 示例：展示标准化后的数据前五行

# 观察年龄与糖尿病患病程度的关系
sns.lmplot(x='age', y='target', data=df, scatter_kws={'alpha': 0.5})
plt.title('Age vs. Diabetes Target')
plt.show()

# 尝试三维可视化（注意：GitHub README.md不支持3D图形显示）
try:
    from mpl_toolkits.mplot3d import Axes3D

    fig = plt.figure(figsize=(8, 6))
    ax = fig.add_subplot(111, projection='3d')

    ax.scatter(df['age'], df['bmi'], df['target'], alpha=0.5)
    ax.set_xlabel('Age')
    ax.set_ylabel('BMI')
    ax.set_zlabel('Target')
    plt.show()
except ImportError or RuntimeError:  # GitHub无法显示3D图形，所以此代码块在README中仅作为参考
    print("请注意：由于GitHub限制，此处无法直接展示3D图像。")

# 分别针对每个特征与年龄组合进行二维线性回归可视化
for feature in df.columns[:-1]:
    if feature != 'age':
        sns.lmplot(x='age', y='target', hue=feature, data=df, scatter_kws={'alpha': 0.5}, height=6)
        plt.title(f'Age vs. Target with hue by {feature}')
        plt.show()
```
