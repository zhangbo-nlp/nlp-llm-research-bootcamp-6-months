# 大语言模型方法与评测

## 本周定位

本周建立对现代大语言模型研究版图的认识。

本周的重点不是训练 LLM，而是理解：大模型如何被使用、如何被对齐、如何被轻量适配、如何结合检索、如何评测。

## 学习主线

1. LLM 基础：decoder-only、next-token prediction、生成参数。
2. Prompting：zero-shot、few-shot、CoT、结构化输出。
3. Post-training：SFT、RLHF、DPO。
4. 轻量适配：LoRA、QLoRA。
5. RAG：检索增强生成。
6. Agent：模型调用工具完成多步任务。
7. 评测：幻觉、偏差、污染、主观评分、prompt 敏感性。

## 建议学习内容

### Prompting

理解概念：

- zero-shot：只给任务说明。
- few-shot：给示例。
- CoT：引导模型展示中间推理。
- 结构化输出：要求 JSON、表格或固定标签。
- prompt 改一点，结果可能明显变化。

### Post-training

理解框架：

```text
pretraining -> SFT -> preference optimization/alignment -> evaluation
```

- SFT：让模型学会按指令回答。
- RLHF：用人类偏好训练 reward model，再优化模型。
- DPO：直接用偏好数据优化模型，比传统 RLHF 更简化。

### LoRA/QLoRA

理解方法：

- 全量微调太贵。
- 冻结大模型，只训练少量低秩参数。
- 适合算力有限下的任务适配。


### RAG 与 Agent

RAG：

```text
文档 -> 切块 -> 检索 -> 拼进 prompt -> 生成答案 -> 检查证据
```

Agent：

```text
目标 -> 思考/规划 -> 调用工具 -> 观察结果 -> 继续行动
```

需要知道二者解决的问题不同：RAG 主要补外部知识，Agent 主要处理多步任务和工具调用。

## 推荐资源

课程/教材：

- Hugging Face LLM Course：LLM、fine-tuning、reasoning models 相关章节。

论文：

- Brown et al., 2020, Language Models are Few-Shot Learners. https://arxiv.org/abs/2005.14165
- Ouyang et al., 2022, Training language models to follow instructions with human feedback. https://arxiv.org/abs/2203.02155
- Hu et al., 2021, LoRA. https://arxiv.org/abs/2106.09685
- Lewis et al., 2020, Retrieval-Augmented Generation. https://arxiv.org/abs/2005.11401
- Yao et al., 2022, ReAct. https://arxiv.org/abs/2210.03629
- 选读：Rafailov et al., 2023, DPO. https://arxiv.org/abs/2305.18290
- 选读：Dettmers et al., 2023, QLoRA. https://arxiv.org/abs/2305.14314
- ...

论文均可借助AI辅助阅读。


## 实践

完成`a4`中的second part，`4. Red-teaming an LLM`不做要求



## 要求

- 一页周报。
- LLM 相关论文阅读摘要一篇。
- `a4`。
