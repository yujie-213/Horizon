---
layout: default
title: "Horizon Summary: 2026-11-17 (EN)"
date: 2026-11-17
lang: en
---

> From 17 items, 6 important content pieces were selected

---

**Technology News**
1. [vLLM v0.34.0 Released with Model Runner V2 Transition and KV Cache Updates](#item-tech-news-1) ⭐️ 8.0/10
2. [Carnegie Mellon Launches Free Computer Science Course Lectures on YouTube](#item-tech-news-2) ⭐️ 8.0/10
3. [Jiff 1.0 Released as a Modern Datetime Library for Rust](#item-tech-news-3) ⭐️ 8.0/10
4. [Optimizely Compromised to Serve Malware on Major Enterprise Websites](#item-tech-news-4) ⭐️ 8.0/10
5. [Marimba: A System One Model for Speech Processing](#item-tech-news-5) ⭐️ 8.0/10
6. [Steering a pretrained music transformer at sampling time into a real-time jazz partner](#item-tech-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vLLM v0.34.0 Released with Model Runner V2 Transition and KV Cache Updates](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 8.0/10

vLLM version 0.34.0 deprecates Model Runner V1 in favor of Model Runner V2 as the sole GPU runner, introduces support for 10 new models including Mistral Large 4 and MiniMax-M3.1-Flash, and enables extensible KV cache by default based on post-warmup free memory. The update defaults block size to 64, requires huggingface\_hub &gt;= 2.0.0, and drops ROCm 7.2 artifacts in favor of ROCm 10.0 images. These changes deliver performance speedups on hardware such as Blackwell and MI355X, though they require migration for existing deployments.

github · khluu · Nov 16, 23:22

**「Background」** vLLM is an open-source LLM serving framework designed to optimize memory management and throughput through techniques like PagedAttention and optimized CUDA kernels.

**「Upgrade and Compatibility Impact」** Operators upgrading to v0.34.0 must remove legacy environment variables such as VLLM\_USE\_V2\_MODEL\_RUNNER, adapt to the new default block size of 64, and update dependencies like huggingface\_hub, tokenizers, and timm. Deployments relying on removed components like Model Runner V1 or older ROCm 7.2 images will fail at startup unless properly reconfigured.

**Tags**: `#artificial intelligence`, `#machine learning`, `#open source`, `#performance optimization`, `#llm serving`

---

<a id="item-tech-news-2"></a>
### [Carnegie Mellon Launches Free Computer Science Course Lectures on YouTube](https://www.cs.cmu.edu/learn/) ⭐️ 8.0/10

Carnegie Mellon University has launched CS Learn to provide free public access to full semesters of its computer science course lectures on YouTube. The initiative relies on student-built production tools to automate the video creation workflow, enabling a small team to release continuous content. Multiple courses are premiering throughout the launch week, with additional courses scheduled to arrive in January.

hackernews · pcompeau · Nov 16, 20:43 · [Discussion](https://news.ycombinator.com/item?id=50522980)

**「Background」** Universities and academic institutions have long experimented with open educational resources, following early pioneering efforts like MIT OpenCourseWare that began publishing lecture materials online decades ago.

**「Impact」** Students and self-taught developers worldwide gain structured, tuition-free access to specialized undergraduate and graduate-level computer science lectures from a top-tier institution.

**「Community Discussion」** Commenters expressed enthusiasm for specific upcoming courses and requested additional core classes, while discussing how mastering foundational computer science remains essential for leveraging AI tools effectively rather than being replaced by them.

**Tags**: `#computer science`, `#education`, `#open source`, `#artificial intelligence`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [Jiff 1.0 Released as a Modern Datetime Library for Rust](https://burntsushi.net/jiff/) ⭐️ 8.0/10

Jiff version 1.0 has been released as a modern datetime library for Rust, developed by burntsushi to address common ecosystem pain points found in alternatives like Chrono. The library provides an alternative API designed around robust datetime handling and usability.

hackernews · burntsushi · Nov 16, 16:53 · [Discussion](https://news.ycombinator.com/item?id=50519744)

**「Background」** Rust developers have historically relied on existing libraries like Chrono for datetime manipulation, which have faced API and maintenance challenges over the years.

**「Community Discussion」** A former Chrono maintainer expressed gratitude for the new library, noting that maintaining legacy APIs often leads to burnout due to resistance against breaking improvements. Commenters praised the project&\#x27;s documentation for clearly outlining its intended use cases and limitations, expressing hope that the ecosystem will widely adopt it.

<details><summary>References</summary>
<ul>
<li><a href="https://burntsushi.net/jiff/">A datetime library for Rust - Andrew Gallant&#x27;s Blog</a></li>

</ul>
</details>

**Tags**: `#rust`, `#software engineering`, `#open source`, `#libraries`

---

<a id="item-tech-news-4"></a>
### [Optimizely Compromised to Serve Malware on Major Enterprise Websites](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

Optimizely suffered a supply-chain security incident that resulted in its infrastructure being compromised to serve malicious JavaScript payloads to high-profile brand websites, including Zoom and GitLab. The injected malware was distributed directly through Optimizely&\#x27;s Content Delivery Network snippets, affecting customer projects as well as Optimizely&\#x27;s own domains such as login.optimizely.com. The exact attack vector granting write access across multiple customer projects remains undisclosed.

hackernews · kristjansson · Nov 16, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50524767)

**「Background」** Web applications frequently rely on third-party JavaScript vendors loaded via remote scripts or tag managers to handle analytics, experimentation, and marketing features. This practice embeds external code directly into the execution context of a host site, exposing visitor sessions to any vulnerabilities or compromises originating upstream from the vendor.

**「Impact」** Organizations relying on third-party vendor scripts face increased security risks and may need to re-evaluate how external code is integrated, monitored, and restricted within their web applications.

**「Community Discussion」** Commenters debated the architectural risks of delegating website script integration to marketing departments without engineering oversight. Participants argued that major publishers should vendor scripts locally or implement stricter release controls, while others noted that tools like NoScript can help reduce exposure to third-party compromises.

**Tags**: `#security`, `#supply-chain`, `#malware`, `#web-development`

---

<a id="item-tech-news-5"></a>
### [Marimba: A System One Model for Speech Processing](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 8.0/10

Charcot AI released Marimba, an open-source speech processing model utilizing a frozen 0.6B Qwen3-ASR encoder paired with lightweight task-specific readouts to evaluate typed questions over 8-second audio windows. The system handles tasks such as zero-shot term spotting, language identification, speaker changes, and speaker counting, matching or outperforming the much larger 30B-A3B Qwen3-Omni on six of nine benchmark tests. However, Marimba does not generalize to unseen tasks like scene classification, where its heads perform at chance level, and it trails specialized baselines on specific datasets such as Smart Turn.

reddit · r/MachineLearning · /u/solanotodesch · Nov 16, 15:47

**「Background」** Speech audio processing typically relies on large end-to-end multimodal models or dedicated single-task architectures to handle diverse analytical queries like speaker diarization and keyword spotting. Marimba approaches this by reusing representations from a frozen automatic speech recognition encoder, avoiding the heavy compute overhead required by larger omni-directional models.

**「Impact」** Developers and researchers can install Marimba via pip, access its Apache-2.0 licensed weights on Hugging Face, or test the live demo to run efficient audio window queries using significantly fewer compute resources than comparable large-scale speech models.

**Tags**: `#artificial intelligence`, `#machine learning`, `#speech recognition`, `#audio processing`, `#open source`

---

<a id="item-tech-news-6"></a>
### [Steering a pretrained music transformer at sampling time into a real-time jazz partner](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

A developer has released &\#x27;duetto&\#x27;, an open-source real-time jazz partner for MIDI keyboards that steers the pretrained Anticipatory Music Transformer at sampling time without fine-tuning. Instead of modifying model weights, a rule layer edits logits before each sample by masking invalid notes and biasing preferred tones, utilizing phrase data from the Weimar Jazz Database. Running on an RTX 3080 Ti, the medium model achieves 12 ms per note and the large model achieves 18 ms per note, while a Jetson Orin Nano runs the large model at approximately 90 ms per note.

reddit · r/MachineLearning · /u/GGAllin43 · Nov 16, 09:19

**「Background」** Music transformers generate symbolic note sequences autoregressively, but controlling their output during live performance typically requires either expensive model fine-tuning or specialized decoding constraints. Steering models at sampling time modifies the logits directly during generation, allowing external rules to guide behavior without retraining the underlying neural network.

**「Impact」** Developers and musicians interested in interactive generative audio can inspect and use the source code for noncommercial purposes, though they may encounter challenges with drift, unpredictability, and balancing the rule layer against model autonomy.

**Tags**: `#Machine Learning`, `#Generative AI`, `#Music Information Retrieval`, `#Transformers`, `#Open Source`

---