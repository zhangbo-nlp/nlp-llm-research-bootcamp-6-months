# 26 周学习目录

| 周次 | 主题 | 主要学习内容 | 主要实践 |
| --- | --- | --- | --- |
| 01 | [Python、Git 与科研习惯](week-01-python-git-research-habits/README.md) | Python 环境、Git、Markdown、科研记录 | 第一个 notebook 和周报 |
| 02 | [Python 数据结构与文本文件](week-02-python-data-structures-files/README.md) | list、dict、函数、文件读写、文本统计 | 文本统计脚本 |
| 03 | [数据分析、必要数学与机器学习入门](week-03-math-linear-algebra-calculus/README.md) | pandas、shape、向量、数据表、样本与标签 | 文本数据分析 notebook |
| 04 | [文本分类 baseline 与评测指标](week-04-probability-statistics-experiments/README.md) | train/dev/test、TF-IDF、Logistic Regression、F1 | 第一个文本分类 baseline |
| 05 | [词表示与文本相似度](week-05-word-representations/README.md) | one-hot、TF-IDF、Word2Vec、GloVe、cosine | 词向量/句向量相似度实验 |
| 06 | [第一阶段小实验](week-06-first-mini-study/README.md) | baseline 对比、错误分析、短报告 | 文本分类小实验与 5 分钟汇报 |
| 07 | [PyTorch 张量与自动求导](week-07-pytorch-tensors-autograd/README.md) | tensor、autograd、loss、optimizer | 梯度下降小练习 |
| 08 | [神经网络文本分类](week-08-neural-text-classification/README.md) | Dataset、DataLoader、embedding、pooling | PyTorch 文本分类器 |
| 09 | [RNN、LSTM 与 GRU](week-09-rnn-lstm-gru/README.md) | 序列、hidden state、门控 | 序列模型小实验 |
| 10 | [Seq2Seq 与生成](week-10-seq2seq/README.md) | encoder-decoder、teacher forcing、解码 | 数字串/字符转换 toy task |
| 11 | [Attention](week-11-attention/README.md) | Q/K/V 直觉、加权求和、Attention 权重 | Attention 小例子 |
| 12 | [Self-Attention 与 Transformer](week-12-self-attention-transformer/README.md) | Self-Attention、Transformer block | 结构图与最小 Self-Attention |
| 13 | [Multi-Head、位置编码与 Mask](week-13-transformer-components/README.md) | 多头、位置、causal mask、残差 | 补全教学版 Transformer 组件 |
| 14 | [Tokenizer 与 Hugging Face](week-14-tokenizers-huggingface/README.md) | subword、input IDs、attention mask、pipeline | tokenizer 分析和模型推理 |
| 15 | [BERT、GPT 与 T5](week-15-pretrained-language-models/README.md) | encoder、decoder、encoder-decoder、预训练目标 | 模型对比表和论文笔记 |
| 16 | [小规模预训练模型微调](week-16-encoder-finetuning/README.md) | Datasets、Trainer、微调、模型评测 | 小型 encoder 文本分类 |
| 17 | [Decoder LLM、生成参数与 Prompt](week-17-decoder-llm-prompting/README.md) | next-token、temperature、zero/few-shot、结构化输出 | 小型 Prompt 对比 |
| 18 | [SFT、RLHF、DPO 与 LoRA](week-18-posttraining-lora/README.md) | 后训练、偏好学习、参数高效微调 | LoRA 参数阅读或小实验 |
| 19 | [检索与 RAG 基础](week-19-retrieval-rag-basics/README.md) | TF-IDF/BM25、embedding、chunk、Hit@k | 小型检索实验 |
| 20 | [RAG 问答与 Agent 入门](week-20-rag-agents/README.md) | 检索增强生成、引用、工具调用、Agent | 带引用的最小 RAG |
| 21 | [LLM 评测、安全与失败分析](week-21-llm-evaluation-safety/README.md) | benchmark、人评、LLM judge、偏差、红队 | 20–30 条小型评测 |
| 22 | [项目选题与计划](week-22-project-question-proposal/README.md) | 研究问题、baseline、指标、范围 | 项目计划与开题汇报 |
| 23 | [项目数据与 baseline](week-23-project-data-baseline/README.md) | 数据准备、划分、最小可运行方法 | baseline 和数据说明 |
| 24 | [项目主实验与对比](week-24-project-main-experiment/README.md) | 只改变一个因素、实验记录 | 主方法和对比结果 |
| 25 | [错误分析与项目报告](week-25-project-analysis-report/README.md) | 错误分类、结果解释、局限、写作 | 最终报告与复现说明 |
| 26 | [展示、答辩与下一步](week-26-project-presentation/README.md) | 汇报、答辩、同伴反馈、学习规划 | 8 页以内 slides 和项目包 |

## 五个阶段检查

- **Week 06**：能完成 TF-IDF 文本分类、结果表和错误分析。
- **Week 11**：能解释 PyTorch 训练循环、序列模型和 Attention。
- **Week 16**：能使用 Hugging Face 完成一次小规模微调。
- **Week 21**：能完成一个 Prompt/RAG 小实验，并说清评测风险。
- **Week 26**：能完成一个小问题、一个 baseline、一个对比和一份报告。
