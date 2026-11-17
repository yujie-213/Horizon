---
layout: default
title: "Horizon Summary: 2026-11-17 (ZH)"
date: 2026-11-17
lang: zh
---

> 从 17 条内容中筛选出 6 条重要资讯。

---

**科技新闻**
1. [vLLM v0.34.0 发布：移除 Model Runner V1 并引入可扩展 KV 缓存默认启用](#item-tech-news-1) ⭐️ 8.0/10
2. [卡内基梅隆大学在 YouTube 上免费提供计算机科学课程](#item-tech-news-2) ⭐️ 8.0/10
3. [Jiff 1.0 发布：面向 Rust 的全新日期时间库](#item-tech-news-3) ⭐️ 8.0/10
4. [Optimizely 供应链遭攻击，向 Zoom 和 GitLab 等知名网站注入恶意软件](#item-tech-news-4) ⭐️ 8.0/10
5. [Marimba：用于语音处理的 System One 模型](#item-tech-news-5) ⭐️ 8.0/10
6. [基于采样时引导的实时爵士乐伴奏系统 Duetto](#item-tech-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [vLLM v0.34.0 发布：移除 Model Runner V1 并引入可扩展 KV 缓存默认启用](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 8.0/10

开源大语言模型推理框架 vLLM 发布 v0.34.0 版本。此次更新彻底移除了 Model Runner V1，将 Model Runner V2 设为唯一的 GPU 运行器，并将可扩展 KV 缓存和 64 的默认块大小（block-size）设为默认配置。新版本新增了对 Mistral Large 4、MiniMax-M3.1-Flash 等 10 款新模型的支持，并在 NVIDIA Blackwell 和 AMD MI355X 等硬件上带来了显著的解码与吞吐量性能提升。

github · khluu · 11月16日 23:22

**「背景介绍」** vLLM 是一个广泛使用的高性能开源大语言模型推理与服务引擎，通过 PagedAttention 等技术优化显存管理。在此之前，其架构中同时维护了 V1 和 V2 两代模型运行器，限制了新硬件特性与复杂并行策略的深度集成。

**「影响与升级注意事项」** 现有用户在升级至 v0.34.0 时需要注意多项重大变更：若配置中包含已移除的 \`VLLM\_USE\_V2\_MODEL\_RUNNER=0\`，系统将在启动时直接报错；同时，默认块大小调整为 64，且对 \`huggingface\_hub &gt;= 2.0.0\` 提出了强制依赖要求。用户可以通过传递 \`--gpu-memory-utilization 0.9\` 或 \`--no-enable-extensible-kv-cache\` 来保留旧版的显存利用和 KV 缓存行为。

**标签**: `#artificial intelligence`, `#machine learning`, `#open source`, `#performance optimization`, `#llm serving`

---

<a id="item-tech-news-2"></a>
### [卡内基梅隆大学在 YouTube 上免费提供计算机科学课程](https://www.cs.cmu.edu/learn/) ⭐️ 8.0/10

卡内基梅隆大学推出了 CS Learn 项目，开始在 YouTube 上免费提供完整学期的计算机科学课程讲座。该项目由学生开发的自动化制作工具支持，首批课程于本周逐日首播，更多课程计划于 1 月份推出。

hackernews · pcompeau · 11月16日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=50522980)

**「背景」** 长期以来，高等院校通过开放在线课程（如 MIT OpenCourseWare）向公众免费分享优质教学资源，但通常需要耗费大量的人力物力进行后期制作。卡内基梅隆大学此次利用学生开发的自动化工具简化了制作流程，使小团队也能完成全套课程的发布。

**「影响」** 全球学习者和开发者可以零成本获取卡内基梅隆大学计算机科学专业的系统性核心课程与前沿讲座，进一步降低了顶尖计算机教育的门槛。

**「社区讨论」** 评论区的校友和学习者对分布式系统、操作系统和田奇灿的机器学习系统等特定课程表达了期待，并讨论了这些基础知识在人工智能时代作为赋能工具而非替代品的重要价值。

**标签**: `#computer science`, `#education`, `#open source`, `#artificial intelligence`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [Jiff 1.0 发布：面向 Rust 的全新日期时间库](https://burntsushi.net/jiff/) ⭐️ 8.0/10

Jiff 1.0 版本已正式发布，这是一个专为 Rust 语言设计的现代化、高质量日期时间库，旨在解决现有生态系统中的痛点。该库由知名开发者 burntsushi 编写，旨在提供更合理的 API 设计与更完善的功能。

hackernews · burntsushi · 11月16日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=50519744)

**「背景」** Rust 生态系统中现有的日期时间库（如 Chrono）在 API 设计、时区处理及防错机制上面临诸多痛点，长期困扰开发者。

**「社区讨论」** 前 Chrono 维护者 quodlibetor 对该库的发布表示感谢，并指出由于历史包袱和维护阻力，旧库的 API 改进空间受限。同时，社区用户对 burntshsi 以往作品的质量表示认可，并期待 Jiff 能够在生态中得到广泛采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://burntsushi.net/jiff/">A datetime library for Rust - Andrew Gallant&#x27;s Blog</a></li>

</ul>
</details>

**标签**: `#rust`, `#software engineering`, `#open source`, `#libraries`

---

<a id="item-tech-news-4"></a>
### [Optimizely 供应链遭攻击，向 Zoom 和 GitLab 等知名网站注入恶意软件](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

第三方服务商 Optimizely 遭到供应链攻击，其系统被黑客利用并向 Zoom、GitLab 以及 Optimizely 自身的官网等知名品牌网站注入了恶意 JavaScript 载荷。攻击者获取了跨客户项目的写入权限，导致受影响的网站通过其 CDN 脚本直接向访问者推送恶意代码。

hackernews · kristjansson · 11月16日 23:00 · [社区讨论](https://news.ycombinator.com/item?id=50524767)

**「背景」** 现代企业广泛通过第三方供应商的脚本（如标签管理器和分析工具）直接将外部代码嵌入其网页中，这绕过了常规的工程审查流程，也带来了巨大的供应链安全隐患。

**「影响」** 依赖第三方 CDN 脚本的组织面临着极高的单点故障和供应链污染风险，即使自身核心基础设施安全，其用户终端也可能遭受恶意代码侵害。

**「社区讨论」** 评论者指出，这种允许营销部门绕过工程团队直接在网站加载外部脚本的做法带来了严重的安全隐患，并呼吁企业重新评估对第三方厂商的盲目信任，采用更严格的发布审核或本地化引入（vendoring）策略。

**标签**: `#security`, `#supply-chain`, `#malware`, `#web-development`

---

<a id="item-tech-news-5"></a>
### [Marimba：用于语音处理的 System One 模型](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 8.0/10

Charcot-AI 推出了 Marimba 语音处理系统，该系统利用冻结的 0.6B ASR 编码器结合专用读出层来回答关于音频窗口的各种问题并返回校准概率。在针对 1,000 个公共问题的测试中，它在 9 个测试中的 6 个上匹配或超越了参数量大得多的 Qwen3-Omni（30B-A3B），并在说话人变化检测和说话人计数基准上分别超越了 ECAPA 和 pyannote 3.1。不过，该模型无法泛化到未见过的任务中，例如在 CochlScene 场景分类中表现处于随机水平，且在轮次结束检测（turn-end detection）上表现落后于 Smart Turn v3.2。官方已在 GitHub 开源相关代码，并在 Hugging Face 上发布了采用 Apache-2.0 许可证的模型权重和在线演示。

reddit · r/MachineLearning · /u/solanotodesch · 11月16日 15:47

**「背景」** 传统的语音理解系统通常依赖于参数量庞大的多模态模型来处理各类音频分析任务，计算开销巨大。而通过冻结小型基础语音编码器并外挂轻量级任务特定读出层，能够在保持高效推理的同时降低资源消耗。

**「影响」** 开发者和研究人员现在可以通过 pip 安装该软件包（marimba-audio），或使用 Apache-2.0 许可证的权重来进行高效的语音问答、术语 spotting 以及说话人分析，同时需注意其在未训练的全新任务上存在泛化能力限制。

**标签**: `#artificial intelligence`, `#machine learning`, `#speech recognition`, `#audio processing`, `#open source`

---

<a id="item-tech-news-6"></a>
### [基于采样时引导的实时爵士乐伴奏系统 Duetto](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

开发者推出了名为 duetto 的实时 MIDI 键盘爵士乐伴奏系统，该系统在无需微调的情况下，通过采样时的规则层直接引导预训练的 Anticipatory Music Transformer 模型。该系统能根据演奏者的输入实时生成伴奏或独奏，在 RTX 3080 Ti 上实现了中型模型 12 毫秒/音符、大型模型 18 毫秒/音符的处理速度。然而，其表现仍存在容易偏离演奏者、响应难以预测以及规则与模型创意之间平衡脆弱的局限性。

reddit · r/MachineLearning · /u/GGAllin43 · 11月16日 09:19

**「背景介绍」** 在生成式音乐领域，传统的模型定制通常依赖于针对特定风格或任务的微调（Fine-tuning），但这会消耗大量计算资源并可能破坏预训练模型的通用能力。近年来，通过在采样阶段直接对模型输出的 Logits 进行掩码和偏置调整（即 Logit 引导或约束解码），研究人员能够在不修改模型权重的前提下实现对生成行为的精确控制。

**标签**: `#Machine Learning`, `#Generative AI`, `#Music Information Retrieval`, `#Transformers`, `#Open Source`

---