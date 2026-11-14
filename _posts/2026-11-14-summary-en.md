---
layout: default
title: "Horizon Summary: 2026-11-14 (EN)"
date: 2026-11-14
lang: en
---

> From 20 items, 4 important content pieces were selected

---

**Technology News**
1. [FAA Issues Nationwide Ground Stop Affecting US Departing Flights](#item-tech-news-1) ⭐️ 8.0/10
2. [Scaling a 1-Trillion Parameter MoE Model on TorchTitan Using 384 GH200 GPUs](#item-tech-news-2) ⭐️ 8.0/10
3. [Frontier AI Models Score Near-Perfect on Materials-Science Test](#item-tech-news-3) ⭐️ 8.0/10
4. [Real-time GPU-accelerated airband monitoring tool captures regional ground stop chatter](#item-tech-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [FAA Issues Nationwide Ground Stop Affecting US Departing Flights](https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247) ⭐️ 8.0/10

The Federal Aviation Administration issued a nationwide ground stop halting departing flights across the United States due to a critical infrastructure issue. The disruption left major airports facing widespread delays and cancellations. Reports indicated potential involvement from a telecommunications network failure and ongoing technical upgrades.

hackernews · zulln · Nov 13, 21:05 · [Discussion](https://news.ycombinator.com/item?id=50489641)

**「Background」** National airspace management relies on centralized telecommunications and radar infrastructure to coordinate safe communication between air traffic controllers and pilots. Disruptions to these foundational radio and data networks can force broad safety halts to prevent hazardous conditions in flight.

**「Impact」** Airlines and travelers nationwide experienced extensive flight delays and cancellations, with airport departure boards showing widespread disruptions and overloaded informational portals.

**「Community Discussion」** Commenters shared developing updates from various news outlets pointing toward potential telecommunications network issues overseen by L3Harris Technologies, while others noted concurrent rollouts of new air traffic control software.

**Tags**: `#infrastructure`, `#aviation`, `#telecommunications`, `#reliability`, `#systems`

---

<a id="item-tech-news-2"></a>
### [Scaling a 1-Trillion Parameter MoE Model on TorchTitan Using 384 GH200 GPUs](https://www.reddit.com/r/MachineLearning/comments/1xvce5h/scaling_to_1t_moe_on_torchtitan_p/) ⭐️ 8.0/10

Engineers scaled a 1-trillion parameter Mixture of Experts \(MoE\) model across 384 GH200 GPUs on the JUPITER supercomputer using TorchTitan, achieving ~1,300 tokens/s per GPU. The setup paired 384-way FSDP with 4-way expert parallelism restricted locally to single nodes, avoiding pipeline parallelism entirely. Key optimizations included offloading activation checkpoints to Grace via the C2C link, switching to Muon optimization with GPU-accelerated Newton-Schulz iterations, and adopting custom sharding and FP8 expert all-gathers to mitigate InfiniBand bottlenecks.

reddit · r/MachineLearning · /u/f14-bertolotti · Nov 13, 16:28

**「Background」** TorchTitan is a native PyTorch library designed for large-scale model training that incorporates modular distributed training components like Fully Sharded Data Parallel \(FSDP\). The JUPITER supercomputer features NVIDIA GH200 Grace Hopper Superchips, which combine an ARM-based CPU and a Hopper GPU linked via a high-speed C2C interconnect, alongside lower-bandwidth InfiniBand networks for inter-node communication.

**「Impact」** AI engineers training frontier-scale MoE models on multi-node GH200 clusters can adopt these TorchTitan configurations—such as stream-aligned allocations using FSDP2 flags and local expert sharding—to eliminate out-of-memory allocator stalls and significantly improve inter-node communication efficiency.

**Tags**: `#Machine Learning`, `#PyTorch`, `#Large Language Models`, `#Distributed Systems`, `#Hardware Acceleration`

---

<a id="item-tech-news-3"></a>
### [Frontier AI Models Score Near-Perfect on Materials-Science Test](https://www.reddit.com/r/MachineLearning/comments/1xvgf6h/four_frontier_models_scored_978100_on_a_7part/) ⭐️ 8.0/10

A researcher evaluated four frontier AI models—Gemini 4 Carbon, Gemini 4 Hydrogen, Claude Opus 5.5, and Claude Fable 5.2—on a rigorous seven-part materials-science technical test. Across 12 fresh runs with web search and code execution enabled, mean scores ranged from 98.5 to 100.0, with all runs completing in 7 to 24 minutes and successfully catching unit traps, hidden CIF tests, and planted manuscript errors. The creator noted that while bounded procedural work is effectively saturated, the results highlight a continuing need for benchmarks that measure open-ended, multi-hour long-horizon agent workflows.

reddit · r/MachineLearning · /u/v\_aravind · Nov 13, 18:58

**「Background」** Standardized evaluations for frontier AI models have increasingly faced benchmark saturation as systems achieve near-perfect marks on static tasks. This has pushed researchers to explore complex multi-step benchmarks like FrontierScience, METR time horizons, and PaperBench to better measure real-world research capabilities.

**Tags**: `#artificial intelligence`, `#machine learning`, `#benchmarking`, `#ai agents`, `#materials science`

---

<a id="item-tech-news-4"></a>
### [Real-time GPU-accelerated airband monitoring tool captures regional ground stop chatter](https://orcasairband.com/) ⭐️ 7.0/10

A developer released a real-time airband radio monitoring tool built using an Ettus B210 software-defined radio paired with a dual-NVIDIA RTX 4090 setup. The system utilizes custom CUDA code to run a polyphase channelizer, capturing and demodulating the entire airband simultaneously while filtering out data transmissions. The tool captured live pilot and air traffic control chatter during an unexpected regional ground stop affecting Victoria, Canada and surrounding airspace.

hackernews · mmaunder · Nov 13, 22:04 · [Discussion](https://news.ycombinator.com/item?id=50490593)

**「Background」** Software-defined radio \(SDR\) hardware converts analog radio frequency signals into digital data streams that can be processed entirely in software. Polyphase channelization is a digital signal processing technique used to efficiently split a wide radio frequency band into many individual narrower communication channels simultaneously.

**「Community Discussion」** Commenters shared unedited transcripts captured by the tool detailing communication issues and ground stop confirmations from Victoria Ground and Vancouver Centre. Participants also discussed the historical prevalence of analog transmissions in aviation for interoperability, and noted parallels to other SDR hobby projects tracking radio signals.

**Tags**: `#software engineering`, `#hardware`, `#cuda`, `#sdr`, `#networking`

---