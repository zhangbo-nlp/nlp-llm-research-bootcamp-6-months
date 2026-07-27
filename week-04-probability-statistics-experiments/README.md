# Week 04 文本分类 Baseline 与评测指标

## 本周定位

本周完成第一个完整的机器学习实验：把文本转成 TF-IDF 特征，再用 Logistic Regression 做分类。

重点不是拿高分，而是理解一个实验的基本结构：数据怎么划分、baseline 为什么重要、指标怎么看、错误样例怎么分析。

如果基础较弱，只要完整跑通一个 TF-IDF 分类器，并能解释每一步，就算合格。

## 本周学习主线

1. 机器学习流程：数据、特征、模型、训练、预测、评测。
2. 数据划分：train、dev、test。
3. 文本表示：Bag-of-Words、n-gram 和 TF-IDF。
4. 分类模型：DummyClassifier 和 Logistic Regression。
5. 指标：accuracy、precision、recall、F1、macro-F1。
6. 混淆矩阵和错误样例。

## 建议学习内容

### 数据划分

重点理解：

- train 用来训练模型。
- dev 用来选择参数和方法。
- test 用来做最后评估。
- 不能看着 test 结果反复改参数。
- 划分后要保存随机种子，后面的模型继续使用同一份划分。

数据很少时，结果会比较不稳定。这不是代码一定写错了，而是需要在报告中说明限制。

### TF-IDF

先理解直觉：

- Bag-of-Words 统计一篇文本里出现了哪些词。
- n-gram 可以保留少量局部顺序。
- TF-IDF 会降低“到处都出现”的词的权重。
- 文本最后会变成一个很宽、但大部分位置都是 0 的稀疏矩阵。

### 评测指标

需要能用自己的话解释：

- accuracy：总体有多少预测正确。
- precision：模型说是某类时，有多少是真的。
- recall：真实属于某类的样本，有多少被找出来。
- F1：precision 和 recall 的综合。
- macro-F1：先算每一类 F1 再平均，类别不均衡时更值得看。

## 推荐资源

- scikit-learn 文本特征文档：https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction
- scikit-learn 模型评测：https://scikit-learn.org/stable/modules/model_evaluation.html
- Google ML Crash Course，Classification：https://developers.google.com/machine-learning/crash-course/classification
- 选读论文：Joulin et al., 2016, Bag of Tricks for Efficient Text Classification：https://arxiv.org/abs/1607.01759

论文只读 Abstract、Introduction 和主结果表，知道“简单方法也可能是强 baseline”即可。

## 本周实践

### 基础实践

- 使用第 3 周数据。
- 划分 train/test，基础较好时再加入 dev。
- 用 `TfidfVectorizer` 提取特征。
- 用 Logistic Regression 训练分类器。
- 输出 accuracy 和 classification report。
- 保存 5 个错误样例。

### 标准实践

在基础实践上补充：

- 加入 `DummyClassifier`。
- 保存 train/dev/test 的样本 ID。
- 输出 macro-F1 和混淆矩阵。
- 比较 unigram 与 unigram + bigram。
- 分析至少 10 个错误样例。

错误可以先分成：

- 文本太短；
- 否定；
- 需要上下文；
- 领域词；
- 标签模糊；
- 可能标错。

### 拓展实践

任选一个：

- 比较 word n-gram 和 character n-gram。
- 多跑 3 个随机种子，看结果是否波动。
- 手工计算一个类别的 TP、FP、FN 和 F1。

## 本周最低要求

- 跑通 TF-IDF + Logistic Regression。
- 能解释 train/test、TF-IDF 和 accuracy。
- 有一个结果表。
- 分析至少 5 个错误样例。

## 本周标准交付

- 一页周报。
- 文本分类代码或 notebook。
- 一个包含 Dummy 和 TF-IDF 的结果表。
- 一张混淆矩阵。
- 10 个错误样例。
- 3 个本周问题。

## 导师检查点

- 学生能否解释为什么需要 baseline？
- 能否说明 TF-IDF 矩阵每一行和每一列是什么？
- 能否解释 accuracy 和 macro-F1 的区别？
- 是否在 test 上反复调参数？
- 错误分析是否指向具体文本？
