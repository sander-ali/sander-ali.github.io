---
layout: page
title: Daily AI news
date: 2025-02-23
description: This page is dedicated to your daily AI news especially related to Agents, LLMs, and Agentic AI
img: assets/img/news/logo_SAK_15.png

images:
  lightbox2: false
  photoswipe: true
  spotlight: false
  venobox: false
---


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/logo_SAK_15.png"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/logo_SAK_15.png" 
           alt="Comapny Logo" 
           style="width: 250px; height: 180px; object-fit: cover; border-radius: 8px;" />
  </div>
</div>

<h1> News 1 </h1>

Are you running open LLMs on Kubernetes? Then you must take a look at AIBrix! AIBrix is ByteDance production solution for open LLMs on Kubernetes running vLLM. 👀 It supports multi-LoRA management, intelligent routing, autoscaling, and fault tolerance

How is AIBrix different from the vLLM production stack?
> AIBrix is an instantiation of what a powerful K8s stack can be and has been in production for the past 6+ months. Production stack is starting from scratch implementation focused on iterating each building block with the feedback and contributions from the community.

TL;DR:
🥳 Has been in production for the past 6+ months at ByteDance across multiple business use cases
💡 High-Density LoRA Management for efficient model adaptation.
🚦 API Gateway and Routing for managing traffic across models.
🛠️ LLM specific Autoscaler (latency/throughput) for dynamic resource scaling.
📦 Sidecar for metric standardization and model management.
💾 Distributed KV Cache for high-capacity, cross-engine KV reuse.
🩺 GPU Hardware Failure Detection for proactive issue identification.

Documentation: https://aibrix.readthedocs.io/latest/
Code: https://github.com/vllm-project/aibrix

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="https://media.licdn.com/dms/image/v2/D4E22AQFlZuYgl8bQjA/feedshare-shrink_800/B4EZUzdeHUHcAg-/0/1740325119829?e=1743033600&v=beta&t=5VYLdjzXvdYPSEPNqLYruzsbH0Xqe20Oj8OLviS3Zzc"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="https://media.licdn.com/dms/image/v2/D4E22AQFlZuYgl8bQjA/feedshare-shrink_800/B4EZUzdeHUHcAg-/0/1740325119829?e=1743033600&v=beta&t=5VYLdjzXvdYPSEPNqLYruzsbH0Xqe20Oj8OLviS3Zzc" 
           alt="Byte Dance" 
           style="width: 250px; height: 180px; object-fit: cover; border-radius: 8px;" />
  </div>
</div>

<h1> News 2 </h1>

The new Google DeepMind Gemini 2.0 Flash lite model supports structured output with Pydantic Models! Thats probably the cheapest and fastest way to convert plain text into a structured format. 👀

🪺 Supports Nested Pydantic models and list
💰 Gemini 2.0 Flash Lite is $0.07/0.30 per million input/output tokens
😍 Available in free tier with 1,500 request per day to test

Code: https://github.com/philschmid/gemini-samples/blob/main/examples/gemini-structured-outputs.ipynb
docs: https://ai.google.dev/gemini-api/docs/structured-output?lang=python

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="https://media.licdn.com/dms/image/v2/D4E22AQEO3kocTf7jdQ/feedshare-shrink_800/B4EZTvPT69GgAg-/0/1739180557438?e=1743033600&v=beta&t=lyN2d0MfeZ8YhHk8RKNjsgAa0Rg6MXXmxjm-LKJXLwk"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="https://media.licdn.com/dms/image/v2/D4E22AQEO3kocTf7jdQ/feedshare-shrink_800/B4EZTvPT69GgAg-/0/1739180557438?e=1743033600&v=beta&t=lyN2d0MfeZ8YhHk8RKNjsgAa0Rg6MXXmxjm-LKJXLwk" 
           alt="Google Gemini 2.0" 
           style="width: 250px; height: 180px; object-fit: cover; border-radius: 8px;" />
  </div>
</div>

<h1> News 3 </h1>

Here are the most popular updates/releases beyond the hype...

📌 xAI 
1. xAI releases Grok 3 claiming to be a powerful agentic model
2. Grok 3 now supports Deepsearch just like OpenAI
- https://x.com/xai/status/1892400129719611567

📌 Github adds new New GPT-4o Copilot code completion model
- https://github.blog/changelog/2025-02-18-new-gpt-4o-copilot-code-completion-model-now-available-in-public-preview-for-copilot-in-vs-code/

📌 Google:
1. Google releases Multi-Agent AI co-scientist
2. Google also releases the PaliGemma 2 Mix
- https://research.google/blog/accelerating-scientific-breakthroughs-with-an-ai-co-scientist/
- https://developers.googleblog.com/en/introducing-paligemma-2-mix/?linkId=13028688

📌 Langchain Introduces MCP Adapters
- https://lnkd.in/gizUDT6W

📌 Sakana AI Launches AI CUDA Enginner
- https://sakana.ai/ai-cuda-engineer/

📌 Microsoft:
1. Microsoft released the most powerful quantum chip named Majorana 1
2. Microsoft Omniparser v2 now allows you to create your opensource computer agent
3. Microsoft releases Muse, an AI model for Gameplay
- https://www.microsoft.com/en-us/research/articles/omniparser-v2-turning-any-llm-into-a-computer-use-agent/
- https://news.xbox.com/en-us/2025/02/19/muse-ai-xbox-empowering-creators-and-players/

📌 Now you can create an AI Agent through Mac's native tools using Apple MCP
- https://github.com/Dhravya/apple-mcp

📌 IBM introduced new AI Integration services to scale AI Agents
- https://newsroom.ibm.com/blog-ibm-introduces-new-ai-integration-services-to-help-enterprises-build-and-scale-ai

📌 BCG Release a report on how to accelerate RnD using AI Agents
- https://media-publications.bcg.com/BCG-Executive-Perspectives-AI-Powered-RandD-EP1-14Feb2025.pdf

📌 PWC report shared how Multi-agent systems are changing businesses
- https://www.pwc.in/assets/pdfs/consulting/technology/emerging-technologies/intelligent-automation/powering-automation-with-agents.pdf

📌 DeeplearningAI drops a new short course on AI Agent observability
- https://www.deeplearning.ai/short-courses/evaluating-ai-agents/

📌 Proxy 1.0 is released as the cheapest alternative to openAI Operator
- https://convergence.ai/?ref=producthunt

📌 Windsurf shares how you can Vibe code better using its turbo mode
- https://x.com/windsurf_ai/status/1891981446698656142

📌 Fireworks AI is now powering Perplexity's Deepresearch features with Deepseek R1
- https://www.linkedin.com/feed/update/urn:li:activity:7298767232434606080/?actorCompanyId=91174981