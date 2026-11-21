---
layout: default
title: "Horizon Summary: 2026-11-21 (ZH)"
date: 2026-11-21
lang: zh
---

> 从 12 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [Levent Alpöge 发布广义黎曼猜想证明及 Lean 形式化代码](#item-tech-news-1) ⭐️ 10.0/10
2. [Navier–Stokes 方程有限时间爆破成果公布](#item-tech-news-2) ⭐️ 10.0/10
3. [陶哲轩讨论无外力纳维-斯托克斯方程奇点与广义黎曼猜想进展](#item-tech-news-3) ⭐️ 10.0/10
4. [Alessandro Masullo 发布 940 页广义黎曼猜想证明草案](#item-tech-news-4) ⭐️ 9.0/10
5. [Thinking Machines 发布开源循环 Transformer 模型 Inkling 2 Mini](#item-tech-news-5) ⭐️ 8.0/10
6. [语言模型研究探讨无需传统训练直接重写自身权重](#item-tech-news-6) ⭐️ 8.0/10
7. [Signal 探讨移动操作系统中集成 AI 带来的隐私与数据捕获风险](#item-tech-news-7) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Levent Alpöge 发布广义黎曼猜想证明及 Lean 形式化代码](https://alpo.ge/remark.pdf) ⭐️ 10.0/10

数学家 Levent Alpöge 宣布与 Anthropic 的 Claude 合作发现了黎曼猜想及广义黎曼猜想的证明。该工作伴随发布了约 1500 万行、解压后达 1.3GB 的 Lean 形式化验证代码。目前相关独立检查（如 MIT 的 Andrew Sutherland 使用 Claude Code 进行的检查）正在进行中。

hackernews · iamronaldo · 11月20日 14:16 · [社区讨论](https://news.ycombinator.com/item?id=50574968)

**「背景信息」** 黎曼猜想是关于黎曼 zeta 函数零点分布的著名未解数学难题，而广义黎曼猜想将其推广到了狄利克雷 L 函数。Lean 是一种交互式定理证明器，能够以机器可检查的严格数学语言对复杂证明进行形式化验证。

**「影响与兼容性」** 如果该证明经数学界全面同行评议和机器验证确认无误，将彻底解决数论及相关数学领域的数百年核心难题，并标志着 AI 在高级数学研究和形式化验证领域取得历史性突破。

**「社区讨论」** Hacker News 评论者对该证明的巨大体量（1.3GB 的分卷压缩 Lean 代码）以及 AI 突破这一数学堡垒的速度感到震惊，同时也引发了对未来人工智能发展及其对科学界深远影响的讨论。

**标签**: `#mathematics`, `#formal verification`, `#lean`, `#number theory`, `#research`

---

<a id="item-tech-news-2"></a>
### [Navier–Stokes 方程有限时间爆破成果公布](https://github.com/tristanbuckmaster/navier-stokes/) ⭐️ 10.0/10

研究人员公开了一项关于 Navier-Stokes 方程有限时间爆破的重要数学研究成果。该成果针对无外力驱动的经典问题进行了探讨，引发了数学界对流体力学基础方程的大量关注与讨论。

hackernews · trotro · 11月20日 15:34 · [社区讨论](https://news.ycombinator.com/item?id=50576232)

**「纳维-斯托克斯方程简介」** 纳维-斯托克斯方程用于描述流体运动，涵盖了从飞机机翼周围的气流、血管内的血流到天气系统、烟雾、波浪和湍流等各种物理现象。

**「社区讨论」** 评论者指出，相比此前借助人为设计外力来破坏方程的成果，这项针对无外力 Navier-Stokes 方程的突破更具现实意义。同时，社区成员也对该成果与近期其他重大数学进展的撞期表示惊叹，并讨论了未来实现物理演示或实时模拟的可能性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.volanea.com/blog/openai-navier-stokes-proof">OpenAI Navier - Stokes Proof: What the AI Claim Means</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#navier-stokes`, `#research`, `#fluid-dynamics`, `#physics`

---

<a id="item-tech-news-3"></a>
### [陶哲轩讨论无外力纳维-斯托克斯方程奇点与广义黎曼猜想进展](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/) ⭐️ 10.0/10

数学家陶哲轩在博客中探讨了流体力学中无外力纳维-斯托克斯方程奇点以及广义黎曼猜想的重大进展。相关成果已通过形式化证明助手验证，并有评论指出得到了两个独立内核的接受。

hackernews · archon1410 · 11月20日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=50578358)

**「背景」** 纳维-斯托克斯方程的奇点问题和黎曼假设长期以来一直是数学界最核心的未解难题，分别关乎流体力学中解的无限性与数论中素数分布规律。

**「社区讨论」** 社区讨论集中在形式化验证的可靠性以及人工智能对科研人员职业生涯的深远影响上。有评论指出，两个独立内核接受该结果意味着 proof 中极少存在内核漏洞，但也有学者对未来人类在科研中的角色和人工智能超越人类智能的趋势感到担忧与不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/">Unforced Euler singularity , unforced Navier - Stokes singularity ...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#artificial intelligence`, `#formal verification`, `#research`

---

<a id="item-tech-news-4"></a>
### [Alessandro Masullo 发布 940 页广义黎曼猜想证明草案](https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/) ⭐️ 9.0/10

Alessandro Masullo 紧急发布了一份长达 940 页的草案，宣称证明了广义黎曼猜想（GRH）。该草案原本计划在斯坦福大学打磨一年后再行公布，但由于面临来自 Anthropic 的竞争性 AI 公告压力，作者选择提前公开当前版本。据数学家 Ravi Vakil 透露，该工作历时 12 年完成，且完全由人类独立推进，此前已接受 Brian Conrad 数个月的密切审查与反馈。

hackernews · jasondavies · 11月20日 18:33 · [社区讨论](https://news.ycombinator.com/item?id=50579568)

**「背景」** 广义黎曼猜想是数学界最著名的未解难题之一，直接关系到数论及相关领域的众多核心性质。由于近年来 AI 在数学推理和复杂证明辅助上的能力迅速提升，人类研究者在重大突破的公布时机上面临着前所未有的外部竞争压力。

**「社区讨论」** 评论者对作者历时 12 年的心血可能被 AI 公告抢先感到惋惜和震惊，并对长达 940 页且尚有未完善细节的草案能否经受住严格检验展开了热烈讨论。部分用户还建议数学界未来应采用加密码哈希和可验证时间戳的方式来明确研究成果的归属。

**标签**: `#mathematics`, `#research`, `#artificial intelligence`, `#community discussion`

---

<a id="item-tech-news-5"></a>
### [Thinking Machines 发布开源循环 Transformer 模型 Inkling 2 Mini](https://thinkingmachines.ai/news/inkling-2-mini/) ⭐️ 8.0/10

Thinking Machines 推出了 Inkling 2 Mini，这是一款采用开源权重的循环 Transformer 模型，其整个训练过程采用 nvfp4 端到端完成。该模型专为本地运行而设计，在基准测试中表现出与更大规模模型相当的性能。

hackernews · jasondavies · 11月20日 20:12 · [社区讨论](https://news.ycombinator.com/item?id=50581260)

**「背景知识」** 传统的 Transformer 模型通常采用固定的前馈层序列进行单向计算。相比之下，循环 Transformer（looped transformer）允许模型在中间层进行循环迭代，从而在不显著增加激活参数的情况下实现更深层次的推理。

**「影响」** 本地用户和开发者在资源受限的硬件（如 AMD Ryzen 和 Apple Silicon 设备）上运行该模型时，可以通过特定的量化或补丁获得可观的生成速度和准确的编码表现。

**「社区讨论」** 社区讨论普遍对其循环架构和端到端 nvfp4 训练持积极态度，并认为其性能表现惊艳。多位用户分享了在本地设备（如 Ryzen 和 M1 Pro 笔记本）上的实测速度与编程测试结果，同时也有人探讨了该架构对未来开源模型设计趋势的潜在示范效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-2-mini/">Introducing Inkling 2 Mini - Thinking Machines Lab</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#machine learning`, `#open source`, `#hardware`

---

<a id="item-tech-news-6"></a>
### [语言模型研究探讨无需传统训练直接重写自身权重](https://arxiv.org/abs/2611.21885) ⭐️ 8.0/10

一篇新研究论文探讨了一种方法，即语言模型通过推理过程而非传统的梯度训练来直接重写自身的权重，在无需传统训练的情况下调整模型。该机制引发了关于其技术实现和潜在局限性的广泛技术讨论。

hackernews · lwhsiao · 11月20日 16:29 · [社区讨论](https://news.ycombinator.com/item?id=50577265)

**「背景」** 语言模型通常依赖基于梯度的传统训练方法来更新其内部权重，以实现性能优化和行为调整。

**「社区讨论」** 评论者指出，模型所谓的自我改进实际效果主要体现在缩短推理轨迹以避免达到 token 限制，并引发了关于这种无梯度自我修改是否应被视为训练形式以及对 AI 安全性的担忧。

**标签**: `#artificial intelligence`, `#machine learning`, `#language models`, `#ai safety`, `#research`

---

<a id="item-tech-news-7"></a>
### [Signal 探讨移动操作系统中集成 AI 带来的隐私与数据捕获风险](https://signal.org/blog/protecting-your-privacy/) ⭐️ 8.0/10

Signal 官方博客发文探讨了移动操作系统深度集成 AI 代理所带来的隐私挑战与数据捕获风险。文章指出系统级 AI 可能会无视应用层面的隐私保护，直接获取用户的敏感聊天内容，甚至通过联系人的设备间接造成数据泄露。

hackernews · dotcoma · 11月20日 09:42 · [社区讨论](https://news.ycombinator.com/item?id=50572348)

**「背景」** 移动操作系统日益集成能够分析屏幕信息的代理式人工智能（Agentic AI），这些系统级工具可能会捕获并存储应用程序内的敏感数据。

**「影响」** 这给依赖应用内隐私保护的用户和开发者敲响了警钟，未来在操作系统原生支持 AI 代理的环境下，即时通讯软件需要采取更底层的技术手段来防止聊天数据被系统级工具抓取。

**「社区讨论」** 社区讨论中，用户对 Signal 应对 AI 威胁的努力表示关注，同时也有评论呼吁公开相关取证调查以造福其他开发者，并讨论了操作系统层面的控制权和验证码等老问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/1038390/signal-blocking-ai-agent-screenshots-mobile-app">Signal is blocking Gemini and Siri AI from reading your... | The Verge</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#privacy`, `#mobile operating systems`, `#security`

---