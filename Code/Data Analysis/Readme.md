```python
```{code-block} python
# 导入所需库
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression, Lasso
from sklearn.metrics import mean_squared_error, r2_score
import numpy as np
import joblib

# 假设已有数据预处理并标准化，变量X_scaled和y已准备就绪

# 划分训练集和测试集
X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.3, random_state=42)

# 线性回归模型
lr_model = LinearRegression()

# 训练线性回归模型
lr_model.fit(X_train, y_train)

# 输出线性回归模型的系数与截距
print("训练后线性回归模型系数: \n", lr_model.coef_)
print("训练后线性回归模型截距项: ", lr_model.intercept_)

# 使用测试集预测结果
y_pred_lr = lr_model.predict(X_test)

# 计算线性回归模型的性能指标
mse_lr = mean_squared_error(y_test, y_pred_lr)
r2_lr = r2_score(y_test, y_pred_lr)

print("\n模型预测性能指标：")
print("Linear Regression - Mean Squared Error: ", mse_lr)
print("Linear Regression - R2 Score: ", r2_lr)

# Lasso 回归模型
lasso_model = Lasso(alpha=1)  # alpha 是正则化强度，实际应用中可能需要调整以优化性能

# 训练 Lasso 回归模型
lasso_model.fit(X_train, y_train)

# 使用测试集预测结果
y_pred_lasso = lasso_model.predict(X_test)

# 计算 Lasso 回归模型的性能指标
mse_lasso = mean_squared_error(y_test, y_pred_lasso)
r2_lasso = r2_score(y_test, y_pred_lasso)

print("\nLasso Regression - Mean Squared Error: ", mse_lasso)
print("Lasso Regression - R2 Score: ", r2_lasso)

# 输出 Lasso 回归模型的系数与截距
print("\nLasso Regression Coefficients: \n", lasso_model.coef_)
print("Lasso Regression Intercept: ", lasso_model.intercept_)

# 保存线性回归模型到本地文件
joblib.dump(lr_model, 'linear_regression_model.pkl')

# 在另一个程序中加载模型（这里仅为演示代码）
# loaded_model = joblib.load('linear_regression_model.pkl')
# y_loaded_pred = loaded_model.predict(X_test)
```
