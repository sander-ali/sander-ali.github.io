---
layout: page
title: Daily AI news
date: 2025-03-08
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

<h1> 8th March 2025 </h1>

<h1> Code Execution from Google DeepMind </h1>

Here is how the Code Execution from Google DeepMind Gemini 2.0 works. Code execution allows Gemini to generate and then run Python code. This enables the model to automatically perform data analysis, algorithmic tasks or solve problems that are difficult or impossible to achieve through text only.

> If the code throws an error it tries to auto-fix, up to 5 times. 

> Supports file input: 1 million tokens = roughly 2MB (e.g. CSV)

> The maximum runtime of the code environment is 30 seconds.

> Python libraries installed: altair, chess, cv2, matplotlib, mpmath, numpy, pandas, pdfminer, reportlab, seaborn, sklearn, statsmodels, striprtf, sympy, and tabulate


Docs: https://ai.google.dev/gemini-api/docs/code-execution?lang=python

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/1.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/1.jpg" 
           alt="Gemini" 
            />
</a>

  </div>
</div>


<h1> AMD introduces Instella</h1>

NEW: AMD introduces Instella, a series of fully open-source, state-of-the-art 3B parameter language models.

It's nice to see AMD pushing out its own small language models. 

It looks like a very competitive model for its size. 

Here's everything you need to know:

• Architecture: Autoregressive transformer with 36 decoder layers and 32 attention heads. This is a text-only model. 

• Sequence Length: 4,096 tokens

• Vocabulary: ~50,000 tokens (using OLMo tokenizer)

• Training Hardware: Installa is trained entirely on AMD Instinct MI300X GPUs; specifically, 128 AMD Instinct MI300X GPUs.

• Multi-Stage Training Pipeline: Stage 1 Pre-training: 4.065 trillion tokens covering diverse content (coding, academic, web). Stage 2 Pre-training: Additional 57.575 billion tokens, including specialized datasets for mathematics, coding, and conversational interactions.

• Supervised Fine-Tuning (SFT): 8.9 billion tokens to enhance instruction-following capabilities. It also includes an alignment Stage (DPO): 760 million tokens for alignment to human preferences (Instella-3B-Instruct).

• Performance Highlights: Instella-3B significantly surpasses existing fully open 3B models (+8.08% average improvement). Competes closely with leading open-weight models like Llama-3.2-3B, Gemma-2-2B, and Qwen-2.5-3B. Achieved outstanding performance improvements in benchmarks like ARC Challenge, MMLU, BBH, and GSM8K. The instruction-tuned models excel in interactive, instruction-following tasks, achieving results comparable to or surpassing open-weight models.

• Training Optimizations: Used FlashAttention-2 for efficient attention computation, Torch Compile for performance acceleration, and Fully Sharded Data Parallelism (FSDP) for optimal resource utilization and scalability.

• Open Source: Fully open-sourced model weights, datasets, training hyperparameters, and code available on Hugging Face and GitHub.

• Future Directions: Plans include expanding context length, enhancing reasoning skills, exploring multimodal capabilities, and scaling up models and datasets.

• License and Usage: Available under a ResearchRAIL license, intended for academic and research purposes only.

Blog: https://rocm.blogs.amd.com/artificial-intelligence/introducing-instella-3B/README.html

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/2.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/2.jpg" 
           alt="OMi" 
            />
</a>

  </div>
</div>


<h1>🔥🔥Distill-Any-Depth: new SOTA MDE🔥🔥</h1>

👉Distill-Any-Depth is the new SOTA monocular depth estimation model trained with a novel knowledge distillation. Source Code, pre-trained models & Hugging Face demo released💙

𝐇𝐢𝐠𝐡𝐥𝐢𝐠𝐡𝐭𝐬:

✅Authors: ZJUT, WestLake University, LZU & NTU

✅Multiple D-normalization on pseudo-label distillation

✅Proposing novel Cross-Context Distillation approach

✅Introducing new multi-teacher distillation framework

✅Pre-trained Models and code released under MIT


👉Paper arxiv.org/pdf/2502.19204

👉Repo https://github.com/Westlake-AGI-Lab/Distill-Any-Depth

🤗Demo https://huggingface.co/spaces/xingyang1/Distill-Any-Depth


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/3.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/3.jpg" 
           alt="Nyx" 
          />
</a>

  </div>
</div>


<h1> How good are ReAct Agents under pressure? </h1>

How good are ReAct Agents under pressure? ReACT (Reasoning and Acting) Agents are AI Agents that combine reasoning with tool calling, enabling them to iteratively think through problems, use tools, and act based on observations to achieve goals. 

LangChain ran benchmarks on far can we push single ReAct Agents by scaling domains (Topic Area, e.g. Customer Support) and available tools.

Results:

🔬 Evaluated Tool calling trajectory (the order of the called tools) and final output with LLM as a Judge.

🦙 Benchmarked Claude 3.5 sonnet, gpt-4o, o1, o3-mini & Llama 3.3 70B

🧠 Both more context and more tools degrade agent performance

📉 Performance on tasks requiring 3+ tool calls dropped more severely than simpler tasks

🛠️ o1, o3-mini, and claude-3.5-sonnet outperform gpt-4o and llama-3.3-70B, .

📅 Calendar Scheduling: o1 (71%) and o3-mini (68%) were top performers with the base domain.

Blog: https://blog.langchain.dev/react-agent-benchmarking/

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/4.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/4.jpg" 
           alt="ClaudeCode" 
           />
</a>

  </div>
</div>

<h1> 🚨 Breaking: Perplexity Launches Voice Mode on macOS </h1>

Perplexity’s latest update brings voice mode to macOS, adding a new way to interact with AI. Now, you can ask questions and get answers—without typing.

🔹Hands-free search for faster results

🔹Switch between voice and text seamlessly

🔹Stay focused without disrupting your workflow

For those who prefer speaking over typing, this update offers a new way to explore ideas and get information.

How do you see voice AI fitting into your daily routine? 🔊

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/5.JPG"
      target="_blank">
      <img src="/assets/img/news/AI news/5.JPG" 
           alt="Gradio" 
          />
</a>

  </div>
</div>

<h1> Exciting news from AMD </h1>

Exciting news from AMD! Thrilled to announce the launch of several new libraries, including our centralized repository: AITER. 

AITER is designed to accelerate AI workloads by supporting a wide range of high-performance AI operators—all in one unified place. This repository is tailored to address various customer operator-level requests, enabling developers to concentrate on crafting operators while customers integrate these collections seamlessly into their own frameworks, whether private, public, or otherwise.

Key Features:

- C++ Level API: Robust support for high-performance computing.

- Python Level API: Easy-to-use interface for rapid development.

- Versatile Kernel Support: Underlying kernels can be sourced from triton, ck, or asm.

- Comprehensive Kernel Coverage: Includes not only inference kernels but also training kernels and GEMM+communication kernels—empowering any kernel+framework combination to overcome architectural limitations.

Proud to support innovation and efficiency in AI development. Check out AITER on GitHub and see how AMD is paving the way for next-generation AI performance!

https://github.com/ROCm/aiter


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/6.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/6.jpg" 
           alt="BirdSQL" 
           />
</a>

  </div>
</div>

<h1> 🚀 Big news for AI agents! </h1>

With the latest release of smolagents, you can now securely execute Python code in sandboxed Docker or E2B environments. 🦾🔒

Here's why this is a game-changer for agent-based systems: 🧵👇

1️⃣ Security First 🔐

Running AI agents in unrestricted Python environments is risky! With sandboxing, your agents are isolated, preventing unintended file access, network abuse, or system modifications.

2️⃣ Deterministic & Reproducible Runs 📦

By running agents in containerized environments, you ensure that every execution happens in a controlled and predictable setting—no more environment mismatches or dependency issues!

3️⃣ Resource Control & Limits 🚦

Docker and E2B allow you to enforce CPU, memory, and execution time limits, so rogue or inefficient agents don’t spiral out of control.

4️⃣ Safer Code Execution in Production 🏭

Deploy AI agents confidently, knowing that any generated code runs in an ephemeral, isolated environment, protecting your host machine and infrastructure.

5️⃣ Easy to Integrate 🛠️

With smolagents, you can simply configure your agent to use Docker or E2B as its execution backend—no need for complex security setups!

6️⃣ Perfect for Autonomous AI Agents 🤖

If your AI agents generate and execute code dynamically, this is a must-have to avoid security pitfalls while enabling advanced automation.

⚡ Get started now: https://github.com/huggingface/smolagents


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/7.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/7.jpg" 
           alt="Selene" 
           />
</a>

  </div>
</div>
