# Week 04 - Probability, Statistics and Experiments

## 本周定位

机器学习实验离不开概率统计。不需要马上掌握严格证明，但必须理解训练集/测试集、均值方差、准确率、混淆矩阵、随机种子和实验可复现。科研里很多错误不是模型错，而是实验设计错。

建议投入：8-12 小时。

## 本周目标

- 理解随机变量、分布、均值、方差、采样。
- 理解训练集、验证集、测试集的不同作用。
- 理解分类任务常见指标：Accuracy、Precision、Recall、F1。
- 能画简单统计图。
- 建立实验日志习惯。

## 理论学习

1. 随机性  
   数据抽样、参数初始化、batch 顺序都会影响结果，因此需要记录随机种子。

2. 数据划分  
   训练集用于学习参数，验证集用于调参，测试集用于最终报告。测试集不能反复调参。

3. 分类指标  
   类别不均衡时，Accuracy 可能误导；需要看 Precision、Recall 和 F1。

4. 统计结论  
   单次实验结果不一定可靠，最好多次运行或至少分析错误样本。

## 工具学习

- NumPy 随机数：`np.random.default_rng`。
- pandas 基础表格操作。
- scikit-learn 指标：`train_test_split`、`classification_report`、`confusion_matrix`。
- Matplotlib 或 seaborn 画柱状图、直方图。

## 推荐资料

- pandas getting started：https://pandas.pydata.org/docs/getting_started/intro_tutorials/
- scikit-learn model evaluation：https://scikit-learn.org/stable/modules/model_evaluation.html
- Google ML Crash Course, Classification：https://developers.google.com/machine-learning/crash-course/classification
- Google ML Crash Course, Training and Test Sets：https://developers.google.com/machine-learning/crash-course/training-and-test-sets/splitting-data

## 实践任务

1. 制作一个带标签的小数据集  
   将第 2 周的 30 条文本扩展到至少 80 条，并为每条标注一个标签，例如：
   - `positive`
   - `negative`
   - `neutral`

2. 数据统计  
   使用 pandas 读取数据，输出：
   - 总样本数。
   - 每个类别数量。
   - 文本长度均值、最大值、最小值。
   - 类别分布柱状图。

3. 数据划分  
   使用 scikit-learn 将数据分成训练集、验证集、测试集，比例建议 70/15/15。记录随机种子。

4. 指标计算
   给定一个小型预测结果表，计算TP、FP、FN、Precision、Recall、F1指标。

5. 实验日志  
   使用 `templates/experiment_log_template.md` 记录本周数据统计实验。

## 最低要求

- 能解释训练集和测试集的区别。
- 能计算 Accuracy 和 F1。
- 能用 pandas 读取 CSV。
- 能保存一张图。

## 挑战任务

- 尝试分层抽样，保证每个集合类别分布接近。
- 人工检查 10 条可能标错的数据，并修正。
- 写一段说明：为什么小数据集结果不稳定。

## 验收标准

- 数据文件包含文本和标签两列。
- 图表清楚展示类别分布。
- 实验日志记录随机种子、数据路径和输出结果。

## 自测问题

1. 为什么测试集不能用于选择模型？
2. 类别极度不均衡时，Accuracy 为什么可能很高但模型没用？
3. Precision 和 Recall 哪个更适合“垃圾邮件拦截”？
4. 为什么要保存原始数据和清洗后数据？
