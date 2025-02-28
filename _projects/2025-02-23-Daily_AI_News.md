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

<h1> 28th February 2025 </h1>

<h1> Microsoft released Phi-4 </h1>

Phi-4 mini update! Microsoft released Phi-4 mini Instruct (3.8B) and Phi-4 Multimodal Instruct (5.6B) with audio and image support by integrating modality-specific LoRAs while keeping the base language model entirely frozen.

Multimodal TL;DR:

🖼️ Understands text, images, and audio in 23 different languages

🌐 Uses a novel "Mixture-of-LoRAs" approach for multilinguality

🧠 5.6B parameter model trained on 5T tokens, 2.3M speech hours, and 1.1T image-text tokens

🥇 #1 on Hugging Face OpenASR leaderboard for speech recognition (better than whisper).

🤗 MIT License and on Hugging Face

✨ Paper teasers a Phi-4-Mini reasoning version

Models: https://huggingface.co/collections/microsoft/phi-4-677e9380e514feb5577a40e4

Paper: https://huggingface.co/microsoft/Phi-4-multimodal-instruct/blob/main/phi_4_mm.tech_report.02252025.pdf

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/1.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/1.jpg" 
           alt="Phi-4" 
            />
</a>

  </div>
</div>


<h1> DeepSeek's 4th Release </h1>

DeepSeek's 4th release - this time 3 repos! One for DualPipe, which aims to overlap communication and computation better. Another for expert parallel load balancing and the other having data for their communication / computation overlap.

DualPipe repo: https://github.com/deepseek-ai/DualPipe.

Load balancing: https://github.com/deepseek-ai/eplb

Data profiler: https://github.com/deepseek-ai/profile-data

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/2.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/2.jpg" 
           alt="DeepSeek" 
            />
</a>

  </div>
</div>


<h1>The Rise of NVIDIA</h1>

AI doesn't stop! NVIDIA just smashed expectations yet again, posting a record $130.5 billion in revenue for the year 😳

Key Q4 2024 financial highlights:

- NVIDIA reported quarterly revenue of $39.3B (+12% increase from the previous quarter & a 78% increase Year-over-Year).

- The company achieved a GAAP EPS of $0.89, beating analyst forecasts of $0.85 (+14% QoQ & +82% YoY).

- Data center revenue hit a record $30.8B (+112% YoY). This growth is driven by strong demand for NVIDIA’s Hopper and Blackwell AI platforms.

We can remember that the DeepSeek AI model from China has raised big concerns about reduced demand for high-end GPUs, which led to a significant market cap drop for NVIDIA last month.

It's now clear that's not the case.

In fact, Nvidia's CEO Jensen Huang just said the opposite is going to happen.

"The next generation of AI will need 100x more compute than older models as a result of new reasoning approaches that think “about how best to answer” questions step by step" - Jensen Huang

AI continues to eat the world, and all roads still lead to NVIDIA.


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/3.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/3.jpg" 
           alt="NVIDIA" 
          />
</a>

  </div>
</div>


<h1> Chain-of-Draft </h1>

Say goodbye to Chain-of-Thought.

Say hello to Chain-of-Draft.

To address the issue of latency in reasoning LLMs, this work introduces Chain-of-Draft (CoD).

Read on for more:

What is it about?

CoD is a new prompting strategy that drastically cuts down verbose intermediate reasoning while preserving strong performance.

Minimalist intermediate drafts

Instead of long step-by-step CoT outputs, CoD asks the model to generate concise, dense-information tokens for each reasoning step. 

This yields up to 80% fewer tokens per response yet maintains accuracy on math, commonsense, and other benchmarks.

Low latency, high accuracy

On GSM8k math problems, CoD achieved 91% accuracy with an 80% token reduction compared to CoT. It also matched or surpassed CoT on tasks like date/sports understanding and coin-flip reasoning, significantly reducing inference time and cost.

Flexible & interpretable

Despite fewer words, CoD keeps the essential logic visible, similar to how humans jot down key points instead of full explanations. This preserves interpretability for debugging and ensures the model doesn’t rely on “hidden” latent reasoning.

Thoughts:

By showing that less is more, CoD can serve real-time applications where cost and speed matter. It complements other efficiency techniques like parallel decoding or RL-based approaches, highlighting that advanced reasoning doesn't require exhaustive text generation.

Paper: https://arxiv.org/pdf/2502.18600


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/4.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/4.jpg" 
           alt="COD" 
           />
</a>

  </div>
</div>

<h1>Phi4 Multimodal and mini models </h1>

Announcing Phi-4 multimodal and mini models in Azure AI Foundry!

✨ Phi-4-mini and Phi-4-multimodal will be available through Azure AI Foundry, Hugging Face, the NVIDIA API Catalog, with an MIT License, allowing for commercial use:

🥇 Phi-4-multimodal (5.6B parameters) excels in speech recognition, translation, summarization, audio understanding, and image analysis. It supports multiple languages (English, Chinese, German, French, Italian, Japanese, Spanish, and Portuguese) and performs strongly in advanced reasoning tasks, particularly in mathematics and logic.

🥈 Phi-4-mini (3.8B parameters) is designed for speed and efficiency. Like the multimodal variant, it excels in text-based reasoning, math, coding, instruction following, and function-calling tasks.

More details at https://azure.microsoft.com/en-us/blog/empowering-innovation-the-next-generation-of-the-phi-family/

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/5.JPG"
      target="_blank">
      <img src="/assets/img/news/AI news/5.JPG" 
           alt="Phi4" 
          />
</a>

  </div>
</div>

<h1> Microsoft Research Announces Magma 8B </h1>

🔥 Agents can do anything! Microsoft Research just announced the release of Magma 8B!

Magma is a new Visual Language Model (VLM) with 8B parameters for multi-modal agents designed to handle complex interactions across virtual and real environments; and it's MIT licensed!

Magma comes with exciting new features such as:

- Introduces the Set-of-Mark and Trace-of-Mark techniques for data labeling prior to the fine-tuning

- Leverages a large amount of unlabeled video data to learn the spatial-temporal grounding and planning

- A strong generalization and ability to be fine-tuned for other agentic tasks

- SOTA in different multi-modal benchmarks spanning across UI navigation, robotics manipulation, image / video understanding and spatial understanding and reasoning

- Generates goal-driven visual plans and actions for agentic use cases

Official Post: https://www.microsoft.com/en-us/research/blog/magma-a-foundation-model-for-multimodal-ai-agents-across-digital-and-physical-worlds/

HuggingFace Hub Model Page: https://huggingface.co/microsoft/Magma-8B

Github Repo: https://github.com/microsoft/Magma/

Project Page: https://microsoft.github.io/Magma/

Technical Report: https://huggingface.co/papers/2502.13130

Demo on HuggingFace Spaces: https://huggingface.co/spaces/microsoft/Magma-UI


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/6.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/6.jpg" 
           alt="Magma8b" 
           />
</a>

  </div>
</div>

<h1> Aria Gen 2 by Meta </h1>

Introducing Aria Gen 2, the next generation of glasses from Meta's Project Aria that we hope will enable researchers across industry and academia to unlock new work in machine perception, egocentric & contextual AI, robotics and more.

More details on what Aria Gen 2 can do ➡️ https://www.meta.com/en-gb/blog/project-aria-gen-2-next-generation-egocentric-research-glasses-reality-labs-ai-robotics/

Get updates on device availability ➡️ https://docs.google.com/forms/d/e/1FAIpQLSfukXP5q6dclAAA3php-OCO1TcwFc5Opegrvw23wHwEbOFJbA/viewform

Highlights for researchers

• State-of-the-art sensor suite featuring an RGB camera, 6DOF SLAM cameras, eye tracking cameras, spatial microphones, IMUs, barometer, magnetometer, and GNSS + a new PPG sensor (heart rate) and contact microphone. 

• Ultra low-power and on-device machine perception for SLAM, eye tracking, hand tracking, and speech recognition using Meta’s custom silicon.

• Capable of six to eight hours of continuous use.

• Open-ear force-canceling speakers, enabling user-in-the-loop system prototyping.

We’re excited to see how researchers at Meta and beyond will leverage Aria Gen 2 to pave the way for future innovations that will shape the next computing platform.

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/7.jpg"
      target="_blank">
      <img src="/assets/img/news/AI news/7.jpg" 
           alt="Aria" 
           />
</a>

  </div>
</div>

<iframe
    src="https://<space-subdomain>.hf.space"
    frameborder="0"
    width="850"
    height="450"
></iframe>