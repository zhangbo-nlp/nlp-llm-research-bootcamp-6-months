# PyTorch、序列建模与 Attention

## 本周定位

本周开始进入深度学习 NLP。对基础一般的学生来说，本周最重要的不是从零写复杂 Seq2Seq，而是理解 PyTorch 训练流程、张量 shape、序列建模的动机，以及 Attention 的直觉。

## 本周学习主线

1. PyTorch 基础：tensor、Dataset、DataLoader、loss、optimizer。
2. 神经网络文本分类：embedding + pooling + classifier。
3. 序列建模：RNN、LSTM、GRU 的直觉。
4. Seq2Seq：encoder-decoder 的输入输出。
5. Attention：为什么 decoder 需要看输入的不同位置。

## 建议学习内容

### PyTorch 基础

需要理解训练循环：

```text
取 batch -> forward -> 计算 loss -> backward -> optimizer.step -> 清空梯度
```

重点能解释：

- `input_ids` 是什么。
- embedding 层做了什么。
- logits 是什么。
- loss 为什么可以指导模型更新。

### 序列建模

理解即可，不要求推导复杂公式：

- RNN 用 hidden state 逐步读序列。
- LSTM/GRU 用门控缓解长期依赖问题。
- Seq2Seq 用 encoder 读输入，用 decoder 生成输出。
- 训练时可以用 teacher forcing，推理时模型依赖自己前一步输出。

### Attention

理解核心直觉：

- 普通 Seq2Seq 把输入压成一个固定向量，长序列容易丢信息。
- Attention 让 decoder 每一步选择性关注输入的不同位置。
- Attention 权重可以可视化，但不能完全等同于“模型理解”。

## 推荐资源

课程/教材：

- PyTorch Tutorials：tensor、autograd、classification 入门。
- CS224N：RNN、Seq2Seq、Attention 相关讲义。

论文：

- Sutskever et al., 2014, Sequence to Sequence Learning with Neural Networks. https://arxiv.org/abs/1409.3215


## 实践

完成 `a2`


## 本周标准交付

- 一页周报。
- Sutskever 论文阅读笔记。
- 完成的`a2`。

