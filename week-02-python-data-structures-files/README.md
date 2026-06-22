# Week 02 - Python Data Structures and Files

## 本周定位

本周继续打 Python 基础，尤其是列表、字典、函数、文件读写和简单文本处理。这些内容会贯穿后续所有 NLP 实验。对零基础学生来说，能把文本文件读进来、清洗、统计、保存，就是进入 NLP 的第一步。

建议投入：8-10 小时。

## 本周目标

- 熟悉列表、元组、字典、集合的使用场景。
- 能编写函数处理文本列表。
- 能读取 `.txt`、`.csv`、`.json` 文件。
- 能用异常信息定位简单 bug。
- 初步理解“数据清洗”和“数据格式”。

## 理论学习

1. 数据结构  
   列表适合有序集合，字典适合键值映射，集合适合去重和成员判断。

2. 函数设计  
   理解输入、输出、副作用、命名、返回值。不要把所有代码写在一个单元格里。

3. 文件与编码  
   理解 UTF-8、换行符、相对路径、绝对路径。

4. 文本处理直觉  
   文本不是“自然就干净”的数据。大小写、标点、空格、乱码、重复样本都会影响实验。

## 工具学习

- Python 标准库：`pathlib`、`json`、`csv`、`collections.Counter`。
- Jupyter notebook 的 markdown 单元与代码单元。
- VS Code 中的运行和调试。
- Git 分支基础：创建分支、切换分支、合并分支。

## 推荐资料

- Python 官方教程第 5-8 章：https://docs.python.org/3/tutorial/
- Python 标准库文档：https://docs.python.org/3/library/
- Pro Git Branching：https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell
- NLTK Book Chapter 1：https://www.nltk.org/book/ch01.html

## 实践任务

1. 制作一个小文本数据集  
   自己收集 30 条中文或英文短句，保存为 `data/week02_sentences.txt`。每行一句。主题可以是课程评价、电影评论、学习感受。

2. 编写文本统计脚本  
   文件名：`notebooks/week02_text_stats.ipynb` 或 `scripts/week02_text_stats.py`。实现：
   - 读取文本文件。
   - 统计句子数量。
   - 统计每条句子的字符数和词数。
   - 输出最长的 5 条句子。
   - 统计最常见的 20 个字符或词。

3. 保存结果  
   输出 `outputs/week02_stats.json`，包含：
   - `num_sentences`
   - `avg_length`
   - `top_tokens`
   - `longest_examples`

4. 写函数并测试  
   至少写 3 个函数：
   - `load_lines(path)`
   - `normalize_text(text)`
   - `count_tokens(lines)`
   每个函数都要用 1-2 个例子验证。

## 最低要求

- 能读取和保存文本文件。
- 能解释列表和字典的区别。
- 能把重复代码改成函数。

## 挑战任务

- 把中文分词和英文空格切词的结果做对比。
- 用命令行参数传入文件路径。
- 使用 `pytest` 给一个函数写测试。

## 验收标准

- 脚本或 notebook 不依赖硬编码绝对路径。
- 输出文件能重新打开并解释字段含义。
- 周报中记录至少一个文件路径或编码相关问题。

## 自测问题

1. 为什么字典查找通常比列表遍历更适合做词频统计？
2. `return` 和 `print` 的区别是什么？
3. 为什么文本数据要保留原始版本？
4. 中文文本和英文文本在“词”的定义上有什么差异？
