---
layout: default
title: "Horizon Summary: 2026-11-25 (ZH)"
date: 2026-11-25
lang: zh
---

> 从 5 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [OpenAI 预印本论文称矩阵乘法指数为九分之四](#item-tech-news-1) ⭐️ 10.0/10
2. [Ternary Bonsai 2.5 27B 模型发布与本地推理表现](#item-tech-news-2) ⭐️ 8.0/10
3. [GPT-6 模型展示内在蛋白质设计能力](#item-tech-news-3) ⭐️ 8.0/10
4. [大语言模型在过去一年中的三个技术拐点](#item-tech-news-4) ⭐️ 8.0/10
5. [GPT-6.2 Astra 自主破解耶鲁大学馆藏 1808 年历史速写本之谜](#item-tech-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 预印本论文称矩阵乘法指数为九分之四](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 10.0/10

OpenAI 发布的一篇数学预印本论文称，已将矩阵乘法指数确定为九分之四（即 $\\Theta\(n^\{2.25\}\)$），并在所有域上证伪了该指数等于 2 的猜想。该论文还声称解决了斯梅尔第九问题（强多项式线性规划）以及平均收益博弈和奇偶博弈等多项数学难题。

hackernews · E-Reverance · 11月25日 01:19 · [社区讨论](https://news.ycombinator.com/item?id=50637220)

**「背景」** 矩阵乘法指数问题旨在寻找用最少运算次数计算矩阵乘法的渐近复杂度下限，长期以来是理论计算机科学的核心开放问题之一。此前学术界对该指数的上下界进行了数十年的持续探索和改进。

**「社区讨论」** 评论指出该预印本来自尚未公开的模型，且具体方法和配方尚未披露。部分讨论认为这表明研发资源正向内部基础数学研究倾斜，但也有观点提醒需谨慎对待未经同行评议的预印本结果。

**标签**: `#artificial intelligence`, `#computer science`, `#mathematics`, `#algorithms`, `#research`

---

<a id="item-tech-news-2"></a>
### [Ternary Bonsai 2.5 27B 模型发布与本地推理表现](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 8.0/10

PrismML 推出了 Ternary Bonsai 2.5 27B 模型，该模型具备 128k 的上下文窗口，并针对本地推理进行了优化。社区用户实测显示，其在消费级硬件（如 Mac Mini M5 Pro）上使用 Q2 GGUF 量化时，生成速度可达约 22-25 tokens/s，展现出在代理式编程（agentic coding）等长文本任务中的应用潜力。

hackernews · b0m · 11月24日 20:08 · [社区讨论](https://news.ycombinator.com/item?id=50633922)

**「背景」** 该模型的前代版本 Ternary Bonsai 2 于 2026 年 9 月发布，采用三进制权重以实现极小的模型体积与高运行效率。

**「影响」** 对于需要在本地运行大语言模型的开发者而言，该模型提供了兼顾高上下文容量与实用生成速度的轻量级选择，有望在本地端支撑更复杂的批量代码编写和代理任务。

**「社区讨论」** 社区用户分享了该模型在硬件上的实测性能数据，并指出其在长视野任务的耗时上较前代版本有所减少。部分评论还探讨了其在基准测试中的表现，并对其能否适应代表性更强的代理式编程任务表达了期待。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/prism-ml/Ternary-Bonsai-2.5-27B-GGUF">prism-ml / Ternary - Bonsai - 2.5 - 27B -GGUF · Hugging Face</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#machine learning`, `#language models`, `#open source`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [GPT-6 模型展示内在蛋白质设计能力](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 8.0/10

OpenAI 的 GPT-6 模型（包括 GPT-6.2）在给定五个靶蛋白的三维结构及结合位点后，能够通过编写代码直接生成潜在微型结合体（minibinder）的三维设计。在实际操作中，研究人员配合使用了 SolubleMPNN 等专用蛋白质 AI 模型来推导氨基酸序列并筛选候选蛋白。该技术展示了前沿大语言模型在计算生物学领域的应用潜力，但也引发了关于其设计实质及实验对照充分性的讨论。

hackernews · acossta · 11月24日 21:02 · [社区讨论](https://news.ycombinator.com/item?id=50634658)

**「背景」** 计算生物学长期依赖专门针对蛋白质结构预测和折叠设计的深度学习模型（如 AlphaFold 等）来处理复杂的分子设计任务。

**「影响」** 科研人员在进行蛋白质设计工作时，可以利用大模型作为协调各专项工具的“黏合剂”，通过编写和调度代码来串联原本独立的生物计算流程，从而提高复杂工作流的构建效率。

**「社区讨论」** 社区讨论主要集中在 GPT-6 在该流程中的实际角色以及实验证据的充分性上。用户 plaidfuji 认为该模型主要起到连接专业工具的“胶水层”作用，而 fabian2k 则对氨基酸序列仍需依赖专业模型 SolubleMPNN 生成这一点提出了设计本质上的疑问；此外，joe-esquibel 指出相关证据偏向计算探索而缺乏实验室生物对照。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/">GPT - 6 models demonstrate intrinsic protein - design ... | OpenAI</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#machine learning`, `#computational biology`, `#software engineering`, `#ai models`

---

<a id="item-tech-news-4"></a>
### [大语言模型在过去一年中的三个技术拐点](https://simonwillison.net/2026/Nov/24/llm-inflection-points/) ⭐️ 8.0/10

过去十二个月中，大语言模型和编码代理经历了三个重大能力拐点：2025 年 11 月发布的 Claude Opus 4.5 与 GPT-5.1 使编码代理达到日常实用水平；2026 年夏季出现的“Fable 级”模型（如 Claude Fable 5）展现出强大的自主问题解决和工具调用能力；随后的 2026 年 9 月至 10 月期间，模型在 3D 建模、空间感知以及游戏玩法设计上取得突破，使 AI 生成的独立游戏具备了真正的娱乐性。

rss · Simon Willison · 11月24日 23:02

**「背景」** 在这些拐点出现之前，早期的编码代理和语言模型由于可靠性不足和缺乏自主纠错能力，往往需要开发人员进行大量人工干预，难以作为日常主力工具。

**「影响」** 软件工程和独立游戏开发领域正面临深度变革，开发者现在可以利用具有自主性的 AI 代理来处理复杂的多系统漏洞、构建 3D 模型并优化游戏玩法，这同时也引发了行业关于 AI 辅助编程的广泛讨论与文化冲突。

**标签**: `#artificial intelligence`, `#software engineering`, `#large language models`, `#coding agents`

---

<a id="item-tech-news-5"></a>
### [GPT-6.2 Astra 自主破解耶鲁大学馆藏 1808 年历史速写本之谜](https://simonwillison.net/2026/Nov/24/astra-historical-mystery/) ⭐️ 7.0/10

历史学家马克·汉弗莱斯（Mark Humphries）分享了一个关于使用 GPT-6.2 Astra 进行历史研究的案例研究。在得到极少提示的情况下，该模型在 22 分钟内利用公开的初级和二级来源，自主识别出了耶鲁大学拜尼克图书馆馆藏的一本 1808 年匿名速写本的创作者。它通过挖掘档案馆中的小众日记线索，准确预测并锁定了证实其假设的维康特·德·夏博（vicomte de Chabot）旅行日志，这一新发现对加拿大及皮毛贸易史具有重要意义。

rss · Simon Willison · 11月24日 16:53

**「背景」** 长久以来，历史研究高度依赖学者在浩瀚的纸质与数字档案中人工搜寻文献、比对碎片化线索。随着大语言模型向具备自主检索与多源推理能力的智能体演进，AI 协助处理复杂档案考证的潜力正逐渐显现。

**「影响」** 这一进展表明，具备自主推理能力的 AI 智能体已经能够协助历史学家完成复杂的跨档案跨源文献考证，并在极短时间内挖掘出未被注意的重要历史文献线索。

**标签**: `#artificial intelligence`, `#historical research`, `#llm agents`, `#case study`

---