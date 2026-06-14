# NLP and LLM Research Bootcamp for First-Year Students

本项目是一套面向完全零基础大一学生的半年科研入门路线，主题聚焦自然语言处理（NLP）与大语言模型（LLM）。默认节奏为 26 周，每周 8-12 小时自学。

## 培养目标

半年结束时，学生应能做到：

1. 熟练使用 Python、Jupyter/Colab、Git、conda/venv、常见数据分析库。
2. 理解机器学习、深度学习、NLP、Transformer、预训练语言模型、RAG、微调和评测的基本概念。
3. 能独立复现一个小型 NLP/LLM 实验，记录实验过程，分析错误案例。
4. 能读懂入门级英文论文的摘要、方法、实验和结论，并写出结构化阅读笔记。
5. 能完成一个小型科研项目：提出问题、找基线、实现实验、做消融/对比、写报告、做展示。

## 使用方式

- 每周进入对应 `week-xx-*` 文件夹，按照 `README.md` 完成理论学习、工具学习、实践任务和交付物。
- 每周至少提交一次学习周报，推荐使用 `templates/weekly_report_template.md`。
- 每读一篇论文，使用 `templates/paper_reading_template.md`。
- 每做一次实验，使用 `templates/experiment_log_template.md`。
- 第 24 周开始使用 `templates/project_proposal_template.md` 和 `templates/final_report_template.md`。

## 建议节奏

| 阶段 | 周数 | 重点 | 结果 |
| --- | --- | --- | --- |
| 基础准备 | 1-4 | Python、Git、数学、概率统计、科研习惯 | 能写简单脚本和周报 |
| 机器学习与传统 NLP | 5-10 | 数据分析、分类、特征、词向量、语言模型 | 能完成文本分类基线 |
| 深度学习与 Transformer | 11-18 | PyTorch、训练流程、Transformer、BERT/GPT、评测 | 能微调和评估预训练模型 |
| LLM 应用与研究技能 | 19-23 | Prompt、语义检索、RAG、PEFT/LoRA、对齐与安全 | 能搭建可测量的 LLM 应用 |
| 小型科研项目 | 24-26 | 选题、复现、实验、报告、展示 | 形成报告、代码和展示材料 |

## 每周固定交付

每位学生每周至少交付：

- 学习周报：本周学了什么、卡在哪里、下周计划是什么。
- 代码或 notebook：哪怕很小，也要能运行。
- 1 页以内概念总结：用自己的话解释本周核心概念。
- 自测问题答案：每周 README 末尾有问题。

小组每周至少交付：

- 一次 5 分钟组内分享。
- 一个可复现记录：代码入口、数据来源、依赖版本、运行结果。

## 学术规范

- 可以使用 ChatGPT、Copilot、通义、Kimi 等工具辅助解释概念、查错和生成草稿，但必须在周报中说明使用方式。
- 不能把 AI 生成内容直接当作自己的理解，必须改写、验证并附上运行结果或推导过程。
- 论文、代码、数据集、模型都必须引用来源。
- 实验报告中必须区分“自己的贡献”和“复用的资源”。

## 推荐硬件与环境

- 初期只需要普通笔记本电脑。
- 深度学习阶段可用 Google Colab、Kaggle Notebook或云服务器。
- 推荐工具：Python 3.12+、JupyterLab 或 VS Code、Git、conda/venv、PyTorch、scikit-learn、Hugging Face Transformers/Datasets/Evaluate。

## 目录说明

- `week-01-*` 到 `week-26-*`：每周学习计划与任务。
- `templates/`：周报、论文阅读、实验日志、开题和结题报告模板。
- `resources.md`：资料索引。
- `project_ideas.md`：适合初学者的科研项目方向。

## AI 辅助说明

本项目在设计、撰写和整理过程中使用了 Codex 等 AI 工具辅助，但所有内容均经过人工审阅和修改。学生在学习过程中也可以合理使用 AI 工具辅助理解和调试，但应记录使用方式，并对自己的学习成果和提交内容负责。
