# Week 05 词表示与文本相似度

## 本周定位

前一周用 TF-IDF 把文本变成了稀疏向量。本周继续学习“文本怎样变成数字”，重点理解从 one-hot、Bag-of-Words、TF-IDF 到 Word2Vec 的变化。

本周不要求自己训练大型词向量。学生需要理解词向量为什么有用，并会用点积和余弦相似度观察词或句子的相似关系。

## 本周学习主线

1. one-hot、Bag-of-Words、TF-IDF。
2. 稀疏向量和稠密向量。
3. 分布式假设：上下文相似的词，含义往往也比较接近。
4. Word2Vec 的基本思路。
5. 点积、向量长度和余弦相似度。
6. 静态词向量的局限：一词多义、未登录词和数据偏差。

## 建议学习内容

### 词表示的发展

建议画一条简单路线：

```text
one-hot
  -> Bag-of-Words
  -> TF-IDF
  -> Word2Vec 
  -> contextual embedding
```

需要说清：

- one-hot 不能直接表示词义相近。
- TF-IDF 更适合表示文档中的词频和重要性。
- 词向量把词放进一个连续空间。
- 静态词向量无法根据上下文改变一个词的表示。

### 余弦相似度

先理解“比较方向是否接近”。本周需要会：

- 计算两个向量的点积。
- 计算向量长度。
- 用 NumPy 实现 cosine similarity。
- 知道相似度高不一定等于语义判断一定正确。

## 推荐资源

- CS224N 2026，Word Vectors 讲义与课程材料：https://web.stanford.edu/class/cs224n/
- Mikolov et al., 2013, Efficient Estimation of Word Representations in Vector Space：https://arxiv.org/abs/1301.3781
- 选读：Pennington et al., 2014, GloVe：https://aclanthology.org/D14-1162/
- 选读：Bojanowski et al., 2016, Enriching Word Vectors with Subword Information：https://arxiv.org/abs/1607.04606

Word2Vec 做本周论文笔记。只读 Abstract、Introduction、方法图/核心思路和主实验表。

## 本周实践

### 基础实践

- 用 NumPy 实现点积、向量长度和余弦相似度。
- 用 5 个手工二维向量检查结果。
- 加载一份小型预训练词向量，或使用现成 embedding 接口。
- 查询 5 个词的近邻词。
- 找 3 个合理结果和 3 个不合理结果。

### 标准实践

在基础实践上补充：

- 准备 30–50 条短句。
- 用平均词向量得到句子表示。
- 给 5 个查询句返回最相似的 3 条句子。
- 与 TF-IDF 相似度结果做简单对比。
- 写一段说明：两种方法分别在哪类例子上更好。

### 拓展实践

- 下载一个现有的 Word2Vec 权重。
- 用 PCA 把 20–30 个词向量画到二维平面。

## 本周最低要求

- 能解释稀疏向量和稠密向量。
- 能手写余弦相似度。
- 完成 5 个词的近邻查询。
- 写一份 Word2Vec 论文笔记。

## 本周标准交付

- 一页周报。
- Word2Vec 论文笔记。
- `week05_word_vectors.ipynb`。
- 6 个成功/失败相似度案例。
- TF-IDF 与词向量的简短对比。
- 3 个本周问题。

## 导师检查点

- 学生能否解释词向量为什么比 one-hot 更容易表示相似关系？
- 能否解释余弦相似度？
- 是否把“向量相似”直接当成“含义完全相同”？
- 能否举出静态词向量处理一词多义失败的例子？
