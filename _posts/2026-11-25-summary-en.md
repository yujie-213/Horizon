---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 5 items, 5 important content pieces were selected

---

**Technology News**
1. [OpenAI Preprint Claims Matrix Multiplication Exponent Is Nine-Fourths](#item-tech-news-1) ⭐️ 10.0/10
2. [Ternary Bonsai 2.5 27B Released for Local Inference](#item-tech-news-2) ⭐️ 8.0/10
3. [GPT-6 Models Demonstrate Intrinsic Protein-Design Capabilities](#item-tech-news-3) ⭐️ 8.0/10
4. [Three LLM Inflection Points Over Twelve Months](#item-tech-news-4) ⭐️ 8.0/10
5. [GPT-6.2 Astra Autonomously Solves an 1808 Historical Sketchbook Mystery at Yale](#item-tech-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Preprint Claims Matrix Multiplication Exponent Is Nine-Fourths](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 10.0/10

An unpeer-reviewed preprint published by OpenAI on GitHub reports establishing the matrix multiplication exponent as nine-fourths, or $\\Theta\(n^\{2.25\}\)$, across every field. The paper also claims to resolve several related long-standing mathematics problems, including Smale&\#x27;s ninth problem on strongly polynomial linear programming, mean-payoff games, and parity games. The specific model and recipe used to generate these results were not disclosed.

hackernews · E-Reverance · Nov 25, 01:19 · [Discussion](https://news.ycombinator.com/item?id=50637220)

**「Background」** The matrix multiplication exponent $\\omega$ represents the infimum of all real numbers $\\nu$ such that multiplying two $n \\times n$ matrices requires $O\(n^\\nu\)$ operations. For decades, researchers have worked to narrow the bounds between the naive $O\(n^3\)$ approach and the theoretical lower limit of $O\(n^2\)$.

**「Community Discussion」** Commenters debated the exact theoretical implications of the preprint, with some noting that the work addresses multiple entries from the Top 500 Open Problems in Math list. Others speculated that the findings reflect internal research efforts using advanced unreleased models.

**Tags**: `#artificial intelligence`, `#computer science`, `#mathematics`, `#algorithms`, `#research`

---

<a id="item-tech-news-2"></a>
### [Ternary Bonsai 2.5 27B Released for Local Inference](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 8.0/10

PrismML has released Ternary Bonsai 2.5 27B, a language model featuring a 128k context window and designed for local inference and agentic coding tasks. The model generates strong community interest for its capability to run efficiently on consumer hardware while supporting extended context lengths.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**「Background」** Ternary quantization uses three weight states \(-1, 0, 1\) to significantly shrink large language model sizes while striving to preserve full-precision accuracy.

**「Impact」** Developers and users can run the model locally using quantized formats like Q2 GGUF, achieving practical token generation speeds and long-context support on hardware such as Apple Silicon Macs for local batch agentic coding.

**「Community Discussion」** Community commenters reported achieving around 22 to 25 tokens per second on a Mac Mini M5 Pro using a Q2 GGUF quantization. Users also noted performance improvements in task completion time compared to earlier versions, alongside discussions regarding its benchmark capabilities relative to larger frontier models.

**Tags**: `#artificial intelligence`, `#machine learning`, `#language models`, `#open source`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [GPT-6 Models Demonstrate Intrinsic Protein-Design Capabilities](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 8.0/10

OpenAI&\#x27;s GPT-6 models have demonstrated intrinsic protein-design capabilities by writing code to create three-dimensional structures for potential minibinders when given target protein structures. To translate these designs into testable proteins, researchers combined GPT-6 with specialized AI models like SolubleMPNN to generate amino acid sequences and filter candidates. Community commenters noted that while the models effectively coordinate specialized tools and write procedural code, the workflow relies heavily on computational exploration with limited wet-lab biological controls presented.

hackernews · acossta · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**「Background」** Protein design traditionally relies on specialized computational biology models and domain-specific tools to generate three-dimensional structures and amino acid sequences.

**「Community Discussion」** Commenters debated whether GPT-6 is performing true novel protein design or acting primarily as an intelligent integration layer that glues together existing specialized computational tools. Users also raised concerns over strict model safety flagging during biological tasks and pointed out a heavy reliance on computational metrics over physical laboratory validation.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/">GPT - 6 models demonstrate intrinsic protein - design ... | OpenAI</a></li>
<li><a href="https://dzen.ru/a/awY4RVfwRRDkTzIS">GPT - 6 .2 сам проектирует белки | AI Новости | Нейросети | Дзен</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#machine learning`, `#computational biology`, `#software engineering`, `#ai models`

---

<a id="item-tech-news-4"></a>
### [Three LLM Inflection Points Over Twelve Months](https://simonwillison.net/2026/Nov/24/llm-inflection-points/) ⭐️ 8.0/10

Over the preceding twelve months, large language models and coding agents crossed three major capability thresholds. In November 2025, models like Anthropic&\#x27;s Claude Opus 4.5 and OpenAI&\#x27;s GPT-5.1 lineup made coding agents reliably accurate for daily development work. In June and July 2026, &\#x27;Fable class&\#x27; models introduced proactive, tool-using autonomy capable of tackling complex, multi-step physical and digital tasks. Finally, in September and October 2026, frontier models like Claude Opus 5.5 mastered 3D modeling, spatial reasoning, and gameplay balancing to produce entertaining indie games from high-level prompts.

rss · Simon Willison · Nov 24, 23:02

**「Background」** Coding assistants and earlier large language models often required constant human intervention and error-correction to handle multi-file tasks or complex debugging. Over the past year, frontier AI labs released increasingly autonomous reasoning models and specialized agents capable of executing broader workflows with minimal hand-holding.

**「Impact」** Developers and creators can now rely on frontier models to autonomously build functioning 3D environments, manage complex multi-system debugging, and iteratively balance game loops. However, this shift is also intensifying industry debates and culture wars around AI-assisted development in indie and commercial game design.

**Tags**: `#artificial intelligence`, `#software engineering`, `#large language models`, `#coding agents`

---

<a id="item-tech-news-5"></a>
### [GPT-6.2 Astra Autonomously Solves an 1808 Historical Sketchbook Mystery at Yale](https://simonwillison.net/2026/Nov/24/astra-historical-mystery/) ⭐️ 7.0/10

History professor Mark Humphries demonstrated that GPT-6.2 Astra autonomously identified the creator of an anonymous 1808 sketchbook at Yale&\#x27;s Beinecke Library in 22 minutes using public primary and secondary sources. The model connected a sketchbook date to a diary reference about the vicomte de Chabot, correctly predicting that an archival journal held at Cleveland State University would confirm the authorship. This physical journal discovery also serves as a significant standalone find for fur trade and Canadian historians.

rss · Simon Willison · Nov 24, 16:53

**「Background」** Yale&\#x27;s Beinecke Rare Book and Manuscript Library holds extensive digitized collections of historical manuscripts, art, and archival materials. Historians frequently rely on cross-referencing disparate primary sources, such as personal diaries and regional library archives, to attribute anonymous works.

**「Impact」** Researchers can leverage agentic AI systems to accelerate archival discovery and solve complex provenance questions across distributed historical collections.

**Tags**: `#artificial intelligence`, `#historical research`, `#llm agents`, `#case study`

---