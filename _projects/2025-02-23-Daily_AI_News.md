---
layout: page
title: Daily AI news
date: 2025-02-25
description: This page is dedicated to your daily AI news especially related to Agents, LLMs, and Agentic AI
img: assets/img/news/logo_SAK_15.PNG

images:
  lightbox2: false
  photoswipe: false
  spotlight: false
  venobox: false
---


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/logo_SAK_15.PNG"
      target="_blank">
      <img src="/assets/img/news/logo_SAK_15.PNG" 
           alt="Comapny Logo" 
           />
</a>

  </div>
</div>

<h1> 27th February 2025 </h1>

<h1> AI Built a civilization on its own </h1>

This is fascinating! Researchers placed 1,000 AI agents in a Minecraft server, and they developed their own civilization with government, culture, and economy 😳

Powered by OpenAI’s o1 model, Altera’s AI agents mimic the human brain with many modules operating in parallel - simulating cognitive functions like attention, memory, and social cognition.

The results? Pretty jaw-dropping.

Left to their own devices, these AI agents:

- Formed alliances: Teaming up to share resources and tackle challenges.

- Built trade networks: Using gems as currency, they bartered goods and services.

- Created governance: Rudimentary laws and leadership structures emerged to maintain order.

- Developed culture: Some agents even crafted rituals, hinting at early forms of religion.

Imagine the potential of models like this at scale, simulating and testing solutions to real-world societal issues.

Soon, global leaders might rely on AI simulations to optimize major decisions before implementation.

Fascinating times.

Source: https://x.com/Rainmaker1973/status/1890637161843593572


<h1> Build Real-time apps with Google DeepMind Gemini </h1>

Want to build Real-time Apps with Google DeepMind Gemini? FastRTC lets you build Python based real-time apps using Gradio-UI. 🔥 

🔄 Transforms Python functions into bidirectional audio/video streams with minimal code

🗣️ Built-in voice detection and automatic turn-taking simplifies conversation interfaces

💻 Supports audio, video, and combined audio-video

🧱 Build with Gradio UI + FastAPI/WebRTC/WebSocket

Gemini Demo (fork and add your api key): https://huggingface.co/spaces/fastrtc/gemini-audio-video

Docs: https://fastrtc.org/advanced-configuration/

Big Kudos to Freddy Boulton from Hugging Face! This make building real time demos with Python really simple!

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/2.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/2.jpg" 
           alt="FastRTC" 
            />
</a>

  </div>
</div>


<h1>Granite LLMs and VLMs</h1>

🔥 Hot of the press: Announcing new Granite LLMs & VLMs! Here's all you need to know:

1/ 𝐆𝐫𝐚𝐧𝐢𝐭𝐞 3.2 𝐈𝐧𝐬𝐭𝐫𝐮𝐜𝐭 (8𝐁 𝐚𝐧𝐝 2𝐁): Introduce chain-of-thought reasoning that can be toggled on/off, significantly improving complex-instruction handling without sacrificing general performance. 

2/ 𝐆𝐫𝐚𝐧𝐢𝐭𝐞 𝐕𝐢𝐬𝐢𝐨𝐧 3.2 2𝐁: A multimodal model focused on document understanding, matching the performance of open models five times its size.

3/ 𝐆𝐫𝐚𝐧𝐢𝐭𝐞-𝐓𝐢𝐦𝐞𝐬𝐞𝐫𝐢𝐞𝐬-𝐓𝐓𝐌-𝐑2.1: Expands TTM forecasting to include daily and weekly predictions alongside the existing minutely and hourly tasks.

4/ 𝐆𝐫𝐚𝐧𝐢𝐭𝐞 𝐆𝐮𝐚𝐫𝐝𝐢𝐚𝐧 3.2: Now features additional model sizes, including a mixture-of-experts (MoE) variant derived from the 3B-A800M language model, offering greater efficiency with minimal performance trade-offs.

5/ 𝐆𝐫𝐚𝐧𝐢𝐭𝐞-𝐄𝐦𝐛𝐞𝐝𝐝𝐢𝐧𝐠-30𝐌-𝐒𝐩𝐚𝐫𝐬𝐞: Adds sparse embedding capabilities to the Granite Embedding series, balancing efficiency and scalability for diverse resource and latency requirements.

All new models are Open Source under the Apache 2.0 license and can be accessed through IBM watsonx.ai, Hugging Face, Ollama, LMStudio, and Replicate.

Get started here: 

- Announcement blog with Benchmarks: https://www.ibm.com/new/announcements/ibm-granite-3-2-open-source-reasoning-and-vision

- Cookbooks: https://github.com/ibm-granite-community/granite-snack-cookbook

- Granite Playground: https://www.ibm.com/granite/playground/

- HuggingFace models: https://huggingface.co/collections/ibm-granite/granite-32-language-models-67b3bc8c13508f6d064cff9a

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/3.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/3.jpg" 
           alt="Granite" 
          />
</a>

  </div>
</div>


<h1> DeepSeek releases DeepEP </h1>

Open-source is on fire. DeepSeek just released DeepEP and it makes large-scale LLMs super fast.

This means better performance for Mixture-of-Experts models without wasting compute.

Here's everything you need to know:

What is Mixture-of-Experts?

MoE models don’t rely on a single massive model. Instead, they use multiple AI "experts" that only activate when needed based on the input. 

How does DeepEP help?

DeepEP helps these experts communicate faster across multiple GPUs, reduces bottlenecks, and makes training and inference much faster. 

It does this using Expert Parallelism (EP). 

What is Expert Parallelism?

EP is the technique that allows these experts to run on separate GPUs at the same time instead of waiting in line. 

This makes MoE models scale efficiently.

Key Features:

▸ Fast GPU communication (153 GB/s inside a machine, 46 GB/s between machines)

▸ Low-latency inference (163 µs response time)

▸ FP8 support for efficient AI computations 

GitHub: https://github.com/deepseek-ai/DeepEP 

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/4.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/4.jpg" 
           alt="DeepEP" 
           />
</a>

  </div>
</div>

<h1>Large Language Diffusion with mAsking </h1>

What is LLaDA and How it is Revolutionizing Language Models with Diffusion?

LLaDA (Large Language Diffusion with mAsking) is a groundbreaking approach to language modeling that departs from traditional autoregressive methods. a diffusion model with an unprecedented 8B scale, trained entirely from scratch, rivaling LLaMA3 8B in performance. 

A text generation method different from the traditional left-to-right approach Instead of generating text sequentially, LLaDA employs a diffusion-based process to predict multiple tokens simultaneously. This innovation enables bidirectional processing and enhances the handling of tasks such as text reversal and reasoning.

Benchmark results reveal that LLaDA performs competitively with models like LLaMA3, positioning it as a promising alternative in the field of large language models.

Blog: https://commitz.vercel.app/articles/llada--revolutionizing-language-models-with-diffusion-1740222154959

Paper: https://arxiv.org/pdf/2502.09992

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/5.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/5.jpeg" 
           alt="LLaDA" 
          />
</a>

  </div>
</div>

<h1> LangChain presents LangGraph Swarm </h1>

🐝 LangGraph Swarm - A lightweight library for building swarm-style multi-agent systems with LangGraph

- Multi-agent collaboration - enable specialized agents to work together and hand off context to each other

- Customizable handoff tools for communication between agents

Watch the video: https://www.youtube.com/watch?v=JeyDrn1dSUQ

Try it out with `pip install langgraph-swarm`

Repo: https://github.com/langchain-ai/langgraph-swarm-py


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/6.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/6.jpg" 
           alt="LangGraph" 
           />
</a>

  </div>
</div>

<h1> Amazon rebuilt Alexa with Generative AI </h1>

Amazon wants to compete with OpenAI ChatGPT and Google DeepMind Gemini App 👀 Amazon just announced Alexa+ a complete refresh of Alexa, here is what we technically know so far:

🚀 Alexa+ will be powered by Amazon Nova and Anthropic Claude

🔗 New “Tool” APIs for 10k+ services & devices, e.g OpenTable, Ticketmaster, Ring, Uber

🤖 Browser use to complete tasks autonomously.

💬 Browser-based experience at Alexa(.)com

⚡ Smart routing with between models for low latency

📰 200+ news sources (AP, Reuters, TIME) for real-time information

🔄 New SDK for building multi-agents to integrate their agents with Alexa+ (not sure what this means).

📚 Integration for document, emails, manuals, recipes.

💰 $19.99/month or free with Prime.

🗓️ Early access in U.S, no info on E.U. access

source: https://www.aboutamazon.com/news/devices/amazon-2025-devices-alexa-event-live-updates

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/7.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/7.jpg" 
           alt="Alexa+" 
           />
</a>

  </div>
</div>