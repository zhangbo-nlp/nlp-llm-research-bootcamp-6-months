# Transformer 与预训练语言模型

## 本周定位

本周进入现代 NLP 的核心：Transformer 和预训练语言模型。本周的目标是理解 Self-Attention、BERT/GPT/T5 的区别，以及 Hugging Face 的基本使用流程。


## 本周学习主线

1. 从 Attention 到 Self-Attention。
2. Transformer block 的组成。
3. 预训练语言模型：BERT、GPT、T5。
4. tokenizer 与模型输入。
5. Hugging Face 基本使用：tokenizer、model、pipeline、简单微调。

## 学习内容

### Transformer

重点理解：

- Self-Attention 让序列内部 token 互相“看见”。
- Multi-Head Attention 让模型在不同子空间学习不同关系。
- Position Embedding/Encoding 提供顺序信息。
- Residual connection 和 LayerNorm 帮助深层模型训练。
- Self-Attention 对长度的复杂度较高，长上下文会更贵。

### 预训练模型

学习BERT、GPT、BART这三个模型方法

可以用一张表理解：

| 类型 | 代表模型 | 结构 | 训练目标 | 适合任务 |
| --- | --- | --- | --- | --- |
| encoder-only | BERT/RoBERTa | 双向 encoder | MLM | 分类、匹配、抽取 |
| decoder-only | GPT/LLaMA/Qwen | 自回归 decoder | CLM | 生成、对话 |
| encoder-decoder | T5/BART | encoder + decoder | text-to-text/denoising | 翻译、摘要、生成式 QA |

### Hugging Face

重点理解这些对象：

- `AutoTokenizer`
- `AutoModel`
- `AutoModelForSequenceClassification`
- `pipeline`
- `datasets`

先会用，再逐步理解内部。

## 推荐资源

课程/教材：

- CS224N：Transformer 相关讲义。
- Hugging Face LLM Course：Transformers、tokenizers、fine-tuning 相关章节。

论文：

- Vaswani et al., 2017, Attention Is All You Need. https://arxiv.org/abs/1706.03762
- Devlin et al., 2018, BERT. https://arxiv.org/abs/1810.04805

本周建议精读 Transformer。BERT，GPT，BART可借助AI进行辅助阅读。

## 实践

### 实践1

Hugging Face 小实验：用小数据跑一次文本分类微调。

数据量可以很小：

- 200-1000 条样本即可。
- epoch 1-2 即可。
- 重点记录流程，不追求高分。

### 实践2

完成 `a3`


## 本周要求

- 一页周报。
- Transformer 论文笔记。
- 一个 Hugging Face 小实验。
- 3 个模型结构对比问题。
- `a3`
