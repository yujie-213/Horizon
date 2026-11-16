---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 17 items, 3 important content pieces were selected

---

**Technology News**
1. [Meta FAIR and NYU Study Finds Vision Encoder Pretraining Optional for MLLMs](#item-tech-news-1) ⭐️ 8.0/10
2. [Making cudaMemcpy 5x Faster on an NVIDIA B300 GPU](#item-tech-news-2) ⭐️ 8.0/10
3. [Protomaps and Affordable Self-Hosted Map Tiles](#item-tech-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Meta FAIR and NYU Study Finds Vision Encoder Pretraining Optional for MLLMs](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Researchers from Meta FAIR and NYU trained over 200 multimodal large language models \(MLLMs\) from scratch under controlled compute budgets to isolate the components of vision encoding. The evaluation reveals that separate encoder pretraining is optional, yielding no performance advantage over training the encoder jointly with the LLM at matched compute. However, vision-only parameters remain strictly necessary; encoder-free models trail across 0.6B to 6.4B scales and require roughly three times the compute to match performance. Furthermore, placing a traditional encoder before the LLM is optional, as an &quot;in-fusion&quot; approach that injects zero-initialized vision-only weights into the LLM&\#x27;s early layers achieves comparable results with reduced latency.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Background」** Contemporary multimodal models diverge widely in their vision architectures, with some adopting standalone pretrained encoders, others training encoders from scratch, and some omitting them entirely. Disentangling the impact of these design choices has remained difficult because published models differ across data distributions, compute scales, and pretraining strategies.

**「Impact」** Developers building MLLMs can reallocate compute away from standalone vision encoder pretraining without sacrificing downstream visual question answering performance, provided the architecture retains dedicated vision-only parameters.

**Tags**: `#artificial intelligence`, `#machine learning`, `#multimodal models`, `#computer vision`, `#research`

---

<a id="item-tech-news-2"></a>
### [Making cudaMemcpy 5x Faster on an NVIDIA B300 GPU](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 8.0/10

A developer released a tuning tool, cudamemcpy-tuner, that accelerates pageable cudaMemcpy transfers by 5x on an NVIDIA B300 GPU. Benchmarks copying a 1 GB tensor demonstrate that the tool raises transfer speeds from 10.2 GB/s to 51.5 GB/s. The repository and accompanying technical blog post are publicly available.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**「Background」** The cudaMemcpy function handles data transfers between host system memory and device GPU memory. Pageable host memory transfers typically achieve lower bandwidth compared to pinned memory because they require staging buffers managed by the operating system.

**「Impact」** Developers and machine learning engineers working with B300 hardware can use the tuner to reduce data transfer bottlenecks during host-to-device and device-to-host operations.

**Tags**: `#CUDA`, `#Hardware`, `#Machine Learning Systems`, `#Performance Optimization`, `#PyTorch`

---

<a id="item-tech-news-3"></a>
### [Protomaps and Affordable Self-Hosted Map Tiles](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

Protomaps and similar modern mapping tools have made self-hosting map tiles inexpensive and accessible for developers and side projects. By leveraging static file storage and client-side rendering, developers can bypass expensive commercial mapping APIs for vector basemaps, though high-resolution satellite imagery remains cost-prohibitive for large-scale self-hosting due to massive storage requirements.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**「Background」** Traditionally, displaying customized interactive maps required either managing complex dedicated tile server infrastructure or paying commercial providers like Mapbox or Google Maps based on request volume. Recent shifts toward single-file archive formats and edge object storage have simplified deploying self-hosted mapping infrastructure.

**「Impact」** Developers running side projects or niche applications can now build map-dependent features affordably by leveraging object storage combined with open-source tile formats.

**「Community Discussion」** Commenters noted that while vector basemaps are cheap to store and serve, high-resolution satellite imagery quickly scales into hundreds of terabytes and becomes expensive. Users also highlighted alternative free public instances like OpenFreeMap and cloud architectures utilizing Cloudflare R2 for privacy and access control.

**Tags**: `#GIS`, `#Open Source`, `#Web Development`, `#Self-Hosting`, `#Mapping`

---