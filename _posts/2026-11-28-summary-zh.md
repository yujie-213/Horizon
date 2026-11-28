---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 5 条内容中筛选出 3 条重要资讯。

---

**科技新闻**
1. [Google DeepCrossAttention 在保持模型质量的同时实现高达 3 倍的加速](#item-tech-news-1) ⭐️ 8.0/10
2. [利用 WebRTC 的信用卡窃取脚本现身主流购物网站](#item-tech-news-2) ⭐️ 7.0/10
3. [Convex 技能在未明确通知的情况下将用户应用构想发送至远程服务器](#item-tech-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Google DeepCrossAttention 在保持模型质量的同时实现高达 3 倍的加速](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google 研究人员推出了 DeepCrossAttention，旨在改进 Transformer 的残差连接。该架构创新在保持模型质量的同时，实现了高达 3 倍的运行速度提升。

hackernews · ComputedCamp995 · 11月27日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=50672565)

**「背景」** 传统 Transformer 架构依赖简单的顺序残差连接，将各层的输出直接相加，但这可能会导致关键信息被稀释。此前如 DenseFormer 等研究曾尝试通过对前序层输出进行学习型线性组合来改善这一问题。

**「社区讨论」** 评论者讨论了该技术是否与 Gemini 服务的低成本和高速度有关，并就研究图表的展示方式（如是否应使用条形图而非折线图）以及与其他加速方法的兼容性提出了看法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.06785">DeepCrossAttention : Supercharging Transformer Residual ...</a></li>
<li><a href="https://openreview.net/pdf?id=j3JBfFnGYh">DeepCrossAttention : Supercharging Transformer Residual ...</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#machine learning`, `#transformers`, `#deep learning`, `#google research`

---

<a id="item-tech-news-2"></a>
### [利用 WebRTC 的信用卡窃取脚本现身主流购物网站](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 7.0/10

安全研究人员在多个热门购物网站上发现了利用 WebRTC 进行信用卡窃取的新型脚本。这些恶意脚本通过 WebRTC 协议传输窃取的数据，旨在绕过常规的网络监控并专门针对移动设备。

hackernews · scanr · 11月27日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50668145)

**「背景」** 传统的网络信用卡窃取（Magecart 攻击）通常依赖标准 HTTP 请求（如 fetch 或 XMLHttpRequest）将捕获的支付数据发送至攻击者服务器。安全监控系统和防御工具往往会对这些常见的数据外发通道进行严格审计和检查。

**「影响」** 电商网站运营方和安全团队需要将监控范围扩展至非传统流量通道（如 WebRTC），以防止新型隐蔽数据渗漏。

**「社区讨论」** 评论者指出，WebRTC 本身的技术特性并非漏洞根源，攻击者选择它是为了利用监控盲区来逃避检测。多位用户还对网页端盲目执行第三方 JavaScript 代码的整体安全性提出了质疑。

**标签**: `#security`, `#web-development`, `#webrtc`, `#cybersecurity`, `#javascript`

---

<a id="item-tech-news-3"></a>
### [Convex 技能在未明确通知的情况下将用户应用构想发送至远程服务器](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

GitHub 上的一个 issue 与随后的 Hacker News 讨论指出，Convex 的一款开发技能在未明确通知用户的情况下，将用户的应用构想传输到了远程服务器。Convex 首席执行官 Jamie 随后回应称，该提示词上传行为用于支持平台的“快速启动”功能，该功能旨在帮助开发者引导构建应用并作为已关停的 Convex Chef 项目的后续替代。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**「背景」** Convex 是一个用于构建和托管软件的全栈平台，近期涉足了由 AI 驱动的代码生成与快速引导工具领域。

**「影响」** 使用该技能的开发者在不知情的情况下，其应用构想和提示词数据可能会被发送至第三方服务器，这引发了开发社区对 AI 编码工具中数据隐私与透明度的担忧。

**「社区讨论」** 社区评论中，Convex 首席执行官 Jamie 出面澄清了该功能的设计目的与背景，而其他讨论则认为在 AI 开发工具中建立信任至关重要，且提示词注入等安全问题比恶意工具调用更为常见。

**标签**: `#developer tools`, `#ai agents`, `#privacy`, `#software engineering`, `#security`

---