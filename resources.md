# 学习资源索引

## 怎么使用这份资源

这份文件是索引，不是“全部必读清单”。

每周先看对应 README，只选择里面指定的 1–2 个主要资源。遇到不懂的概念，再回到这里找补充材料。对学生来说，把一个教程真正看懂、代码真正跑通，比收藏很多课程更有用。

## Python、数据与基础工具

- Python 官方教程：https://docs.python.org/3/tutorial/
- NumPy Quickstart：https://numpy.org/doc/stable/user/quickstart.html
- pandas 入门教程：https://pandas.pydata.org/docs/getting_started/intro_tutorials/
- Matplotlib Quick Start：https://matplotlib.org/stable/users/explain/quick_start.html
- Pro Git 中文版：https://git-scm.com/book/zh/v2
- Google Colab 介绍：https://colab.research.google.com/notebooks/intro.ipynb

适用周次：Week 01–07，以及后续所有实验。

## 机器学习与传统 NLP

- Google Machine Learning Crash Course：https://developers.google.com/machine-learning/crash-course
- scikit-learn User Guide：https://scikit-learn.org/stable/user_guide.html
- scikit-learn 文本特征：https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction
- scikit-learn 模型评测：https://scikit-learn.org/stable/modules/model_evaluation.html
- Speech and Language Processing（第三版草稿）：https://web.stanford.edu/~jurafsky/slp3/

适用周次：Week 03–06。

### 重点论文

- Word2Vec：https://arxiv.org/abs/1301.3781
- GloVe：https://aclanthology.org/D14-1162/
- FastText 文本分类：https://arxiv.org/abs/1607.01759
- FastText 子词词向量：https://arxiv.org/abs/1607.04606

## PyTorch、RNN 与 Attention

- PyTorch Learn the Basics：https://docs.pytorch.org/tutorials/beginner/basics/intro.html
- PyTorch Seq2Seq Tutorial：https://docs.pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html
- Understanding LSTM Networks：https://colah.github.io/posts/2015-08-Understanding-LSTMs/
- Stanford CS224N 2026：https://web.stanford.edu/class/cs224n/

适用周次：Week 07–13。

### 重点论文

- Seq2Seq：https://arxiv.org/abs/1409.3215
- RNN Encoder-Decoder / GRU：https://arxiv.org/abs/1406.1078
- Bahdanau Attention：https://arxiv.org/abs/1409.0473
- Attention Is All You Need：https://arxiv.org/abs/1706.03762

## Transformer 与预训练语言模型

- Hugging Face LLM Course：https://huggingface.co/learn/llm-course/en/chapter0/1
- Transformers 文档：https://huggingface.co/docs/transformers/
- Datasets 文档：https://huggingface.co/docs/datasets/
- Tokenizers 文档：https://huggingface.co/docs/tokenizers/main/index
- The Illustrated Transformer：https://jalammar.github.io/illustrated-transformer/
- The Annotated Transformer：https://nlp.seas.harvard.edu/annotated-transformer/

适用周次：Week 12–16。

### 重点论文

- Transformer：https://arxiv.org/abs/1706.03762
- BERT：https://arxiv.org/abs/1810.04805
- GPT-2 技术报告：https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf
- T5：https://arxiv.org/abs/1910.10683

## LLM、后训练与 Prompt

- Hugging Face Text Generation：https://huggingface.co/docs/transformers/main/en/llm_tutorial
- Hugging Face Chat Templates：https://huggingface.co/docs/transformers/main/en/chat_templating
- Hugging Face PEFT 文档：https://huggingface.co/docs/peft/
- Hugging Face Agents Course：https://huggingface.co/learn/agents-course/

适用周次：Week 17–21。

### 重点论文

- GPT-3 / Few-shot：https://arxiv.org/abs/2005.14165
- InstructGPT / RLHF：https://arxiv.org/abs/2203.02155
- DPO：https://arxiv.org/abs/2305.18290
- LoRA：https://arxiv.org/abs/2106.09685
- QLoRA：https://arxiv.org/abs/2305.14314
- ReAct：https://arxiv.org/abs/2210.03629

## 检索、RAG 与评测

- Sentence Transformers Semantic Search：https://www.sbert.net/examples/sentence_transformer/applications/semantic-search/README.html
- FAISS 文档：https://faiss.ai/
- LlamaIndex RAG Introduction：https://developers.llamaindex.ai/python/framework/understanding/rag/
- Hugging Face Evaluate：https://huggingface.co/docs/evaluate/

小型实验不需要先安装向量数据库。100–500 个文档直接用 NumPy 或 scikit-learn 计算相似度就够了。

### 重点论文

- RAG：https://arxiv.org/abs/2005.11401
- Sentence-BERT：https://arxiv.org/abs/1908.10084
- HELM：https://arxiv.org/abs/2211.09110

## 论文与项目资料

- ACL Anthology：https://aclanthology.org/
- Papers with Code NLP：https://paperswithcode.com/area/natural-language-processing
- arXiv Computation and Language：https://arxiv.org/list/cs.CL/recent
- Hugging Face Papers：https://huggingface.co/papers
- CS224N Project Reports：https://web.stanford.edu/class/cs224n/project.html

## 资料选择建议

遇到一个主题时，优先顺序建议是：

1. 本周 README 的中文说明；
2. 官方教程或课程讲义；
3. 最小代码示例；
4. 论文的摘要、引言、方法图和主结果表；
5. 有余力再看更多推导和扩展阅读。

不要把博客、短视频或 AI 回答当作唯一来源。它们可以帮助理解，但重要概念、API 和论文结论要回到官方文档或原论文核对。
