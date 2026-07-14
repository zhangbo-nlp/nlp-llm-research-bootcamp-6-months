# Week 03 - Math: Linear Algebra and Calculus

## 本周定位

本周补机器学习需要的最低数学基础。不要把目标设成完整学完线性代数和微积分，而是让学生理解向量、矩阵、点积、矩阵乘法、导数、梯度这些概念为什么会出现在模型里。

建议投入：10-12 小时。

## 本周目标

- 理解标量、向量、矩阵、张量的区别。
- 能用 NumPy 创建和操作数组。
- 理解点积、矩阵乘法和相似度的关系。
- 理解导数和梯度下降的直觉。
- 能画出简单函数曲线并观察斜率。

## 理论学习

1. 向量表示  
   文本最终会被表示成数字向量。向量可以代表词、句子、文档或模型参数。

2. 点积与相似度  
   点积可以衡量两个向量方向是否接近，是检索、分类、注意力机制的基础。

3. 矩阵乘法  
   神经网络中的线性层本质上就是输入矩阵乘以权重矩阵再加偏置。

4. 导数和梯度  
   训练模型就是不断调整参数，让损失函数变小。梯度告诉我们参数应该往哪个方向改。

## 工具学习

- NumPy：`array`、`shape`、`reshape`、`matmul`、广播。
- Matplotlib：画函数曲线和散点图。
- notebook 中用 Markdown 写公式说明。

## 推荐资料

- NumPy quickstart：https://numpy.org/doc/stable/user/quickstart.html
- Matplotlib pyplot tutorial：https://matplotlib.org/stable/tutorials/pyplot.html
- 3Blue1Brown Essence of Linear Algebra：https://www.3blue1brown.com/topics/linear-algebra
- Neural Networks and Deep Learning Chapter 1：http://neuralnetworksanddeeplearning.com/chap1.html

## 实践任务

1. NumPy 形状练习  
   创建以下数组并写出 shape：
   - 一个长度为 5 的向量。
   - 一个 3x4 矩阵。
   - 一个 2x3x4 张量。
   - 一个 batch 中 8 条句子、每条 16 个 token、每个 token 64 维向量的张量。

2. 手写相似度计算  
   给定 5 个二维向量，计算两两点积和余弦相似度，用表格展示。

3. 梯度下降直觉实验  
   对函数 `f(x) = (x - 3)^2`：
   - 画出函数曲线。
   - 从 `x = -5` 开始，用手写循环做 20 步梯度下降。
   - 尝试学习率 0.01、0.1、1.0，比较结果。

4. 矩阵乘法解释  
   写一段文字解释：为什么 `(batch_size, input_dim) @ (input_dim, output_dim)` 的结果是 `(batch_size, output_dim)`。

## 最低要求

- 能正确解释 `shape`。
- 能用 NumPy 完成矩阵乘法。
- 能说出梯度下降的直觉。

## 挑战任务

- 手写一个线性回归的梯度下降，不使用 scikit-learn。
- 解释为什么学习率过大可能导致损失不下降。
- 用动画或多张图展示参数更新过程。

## 验收标准

- notebook 中每个数组操作都有 shape 注释。
- 梯度下降实验至少比较 3 个学习率。
- 周报中必须包含一个自己画的图。

## 自测问题

1. 点积大是否一定代表两个向量更相似？
2. 矩阵乘法为什么要求前一个矩阵的列数等于后一个矩阵的行数？
3. 梯度为 0 一定代表找到最优点吗？
4. 为什么神经网络训练需要大量矩阵运算？
