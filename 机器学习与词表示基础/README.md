# 机器学习基础、文本分类与词表示

## 本周定位

本周重点是理解一个 NLP 实验的基本结构，而不是追求复杂模型。学生要知道：数据如何划分、baseline 为什么重要、指标怎么看、错误样例如何分析。

如果学生基础弱，本周只要求完整跑通一个 TF-IDF 文本分类 baseline，并能解释每一步。

## 本周学习主线

1. 机器学习基本概念：样本、标签、特征、模型、损失、指标。
2. 数据划分：train/dev/test。
3. 文本分类 baseline：TF-IDF + Logistic Regression。
4. 词表示：one-hot、TF-IDF、Word2Vec、GloVe。
5. 实验结果解释：accuracy、precision、recall、F1、错误分析。

## 建议学习内容

### 机器学习基础

重点理解：

- baseline 是科研实验的参照物。
- train 用来训练，dev 用来调参，test 用来最终评估。
- 不能在 test set 上反复调参数。
- 单次实验结果可能受随机种子影响。

### 指标

需要能用自己的话解释：

- accuracy：总体预测对了多少。
- precision：预测为某类时，有多少是真的。
- recall：真实属于某类时，有多少被找回来。
- F1：precision 和 recall 的折中。
- macro-F1：类别不均衡时更值得关注。

### 词表示

理解层次即可：

```text
one-hot -> Bag-of-Words -> TF-IDF -> word embedding -> contextual embedding
```

不要求自己训练 Word2Vec，但要理解词向量的核心动机：让语义相近的词在向量空间中更接近。

## 推荐资源

教材/课程：

- CS224N：word vectors 相关讲义。
- scikit-learn 文本特征与分类文档。

论文：

- Mikolov et al., 2013, Efficient Estimation of Word Representations in Vector Space. https://arxiv.org/abs/1301.3781

Word2Vec 论文只要求看 Abstract、Introduction、Model Architectures。

## 实践
完成 `a1`目录中的 exploring_word_vectors.ipynb

## 本周标准交付

- 一页周报。
- Word2Vec 后续论文阅读摘要。
- 补全的 exploring_word_vectors.ipynb
