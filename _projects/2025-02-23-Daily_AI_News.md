---
layout: page
title: Daily AI news
date: 2025-03-26
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

<h1> 26th March 2025 </h1>

<h1> ☄️ GRPO now scales to 70B+ models </h1>

☄️ GRPO now scales to 70B+ models with multi-node training and super-fast performance. Train up to 60 times faster with all the freshest features and optimizations that we've added. More details in the thread below 🧵👇

Install the latest v0.16 version of TRL.

🐦‍🔥 GRPO is now 6x faster with multi-step optimization

This new feature allows for the reuse of generated data across multiple optimization steps, cutting down training time significantly.

TRL added importance sampling and clipping logic to make this possible. Set num_iterations to 4 or more for the full effect!

🩺 Dr GRPO

TRL integrated two major insights from Dr GRPO:

1️⃣ Global normalization to avoid response-level length bias (no more per-sequence normalization).

2️⃣ The option to disable reward scaling to eliminate question-level difficulty bias!

🤸‍♀️ Domain-specific rewards

When optimizing across multiple domains, not all rewards apply to every sample. For example, math rewards shouldn’t be given to biology samples (and vice versa).

Now, you can return None for irrelevant rewards based on the sample's domain!


🍃 Save time and memory with beta=0.0

By setting beta to 0, the reference model is not loaded, and KL divergence is not computed, leading to big savings in memory and compute while still achieving great results!

🕊️ Padding-free batching for SFT

This method reduces memory usage by flattening batches into a single sequence, keeping sequences intact without padding—avoiding cross-contamination seen in packing.

Enable it by setting padding_free=True in SFTConfig.


Increasing the upper bound epsilon, as shown in the DAPO paper, leads to higher entropy during generation, promoting better exploration.

Now, you can easily adjust the upper bound epsilon in GRPO with `epsilon_high` for more diverse outcomes.

More here:

📜 Release notes: https://github.com/huggingface/trl/releases/tag/v0.16.0 

💼 PyPI: https://pypi.org/project/trl/

🐋 OpenR1: https://github.com/huggingface/open-r1


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
     <a href="/assets/img/news/AI news/1.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/1.jpg" 
           alt="Nyx" 
          />
</a>
  </div>
</div>

<hr>
<hr>

<h1> 🔥🔥 Dereflecting Any Image 🔥🔥 </h1>

👉SJTU & Huawei unveils Dereflection Any Image (DAI), novel diffusion-based framework able to recover from a wide range of reflection types. One-step diffusion with deterministic outputs and fast inference. Inference code, pretrained models & training released💙

𝐇𝐢𝐠𝐡𝐥𝐢𝐠𝐡𝐭𝐬:

✅Proposing a novel/efficient pipeline for data collection

✅DRR: HQ dataset w/ diverse reflections w/ varying angles

✅New diffusion-based framework with progressive training

✅SOTA performance also on challenging mobile captures

👉Paper https://arxiv.org/pdf/2503.17347

👉Project https://abuuu122.github.io/DAI.github.io/

👉Repo https://github.com/Abuuu122/Dereflection-Any-Image

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <iframe width="560" height="315" src="https://abuuu122.github.io/DAI.github.io/static/videos/demo.mp4"></iframe>


  </div>
</div>

<hr>
<hr>

<h1> Netflix has built a unified recommendation foundation model </h1>

Netflix has built a unified recommendation foundation model to replace its many specialized systems across their large-scale personalization and recommenders systems internally which drive 80% of the content discovery in their platform. 

Netflix has been able to leverage large-scale high-quality user interaction data together with advanced tokenization techniques (with inspiration from LLMs) to train a foundation model that captures long-term user behavior over extensive interaction histories. 

In their overview they also dive into their cold-start problem, and how they tackle with with a hybrid embedding strategy which combines learnable ID and metadata-based embeddings via an attention mechanism to better handle newly launched titles. 

It is interesting to see that foundation models are now seeing practical applications in growing number of industry applications. 


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

<hr>
<hr>

<h1>  MIT Media Lab researchers just introduced a neuroadaptive AI tutor  </h1>

MIT Media Lab researchers just introduced a neuroadaptive AI tutor that personalizes learning in real time using brainwaves!

Traditional AI tutors rely on static responses, failing to adapt to a learner’s mental state.

𝗡𝗲𝘂𝗿𝗼𝗖𝗵𝗮𝘁 𝗰𝗼𝗺𝗯𝗶𝗻𝗲𝘀 𝗲𝗹𝗲𝗰𝘁𝗿𝗼𝗲𝗻𝗰𝗲𝗽𝗵𝗮𝗹𝗼𝗴𝗿𝗮𝗽𝗵𝘆 (𝗘𝗘𝗚) 𝘄𝗶𝘁𝗵 𝗚𝗣𝗧-𝟰, 𝗺𝗼𝗻𝗶𝘁𝗼𝗿𝗶𝗻𝗴 𝗲𝗻𝗴𝗮𝗴𝗲𝗺𝗲𝗻𝘁 𝗮𝗻𝗱 𝗮𝗱𝗷𝘂𝘀𝘁𝗶𝗻𝗴 𝗰𝗼𝗻𝘁𝗲𝗻𝘁 𝗱𝘆𝗻𝗮𝗺𝗶𝗰𝗮𝗹𝗹𝘆.

1. Tracked real-time brain activity with a wearable EEG headband, measuring cognitive engagement.

2. Modified chatbot responses such as simplifying, elaborating, or changing pacing based on engagement levels.

3. Increased cognitive engagement significantly in a study of 24 participants, outperforming standard AI tutors.

4. Showed no immediate impact on learning outcomes, highlighting the challenge of converting engagement into retention.

Honestly as a student, I could see myself using this haha. Really neat

I see a lot of personalized, AI-driven tutoring applications out there. 

NeuroChat is cool to me because it advances the field by dynamically adjusting content based on real-time physiological data.

Here's the awesome work: https://arxiv.org/abs/2503.07599


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/4.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/4.jpg" 
           alt="Nyx" 
          />
</a>

  </div>
</div>

<hr>
<hr>

<h1> Real-time communication Library to build Voice AI Agents in Python!🔥 </h1>

Turn any python function into a real-time audio and video stream over WebRTC or WebSockets.

Here is how it works:

Simply write a Python function that takes in audio or video data, processes it however you want, and returns the output. FastRTC handles all the complex real-time streaming, including WebRTC and WebSocket connections, so you can focus purely on your logic.

Key Features:

• 🗣 Automatic Voice Detection & Turn-Taking — Focus only on your response logic.

• 💻 Built-in Gradio UI — Instantly launch a WebRTC-enabled interface with .ui.launch().

• 🔌 WebRTC Support — Mount on a FastAPI app with .mount(app) and get a WebRTC endpoint for custom frontends.

• ⚡ WebSocket Support — Expose a websocket endpoint just as easily with .mount(app).

• 📞 Phone Call Support — Spin up a temporary phone number with .fastphone() and handle calls directly.

• 🤖 Customizable Backend — Integrates seamlessly with FastAPI for production-ready applications.

The best part?

It's 100% Open Source

Github Repo: https://github.com/freddyaboulton/fastrtc

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/5.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/5.jpg" 
           alt="Nyx" 
          />
</a>


  </div>
</div>

<hr>
<hr>

<h1> A billion-parameter voice AI is now open source 😳 </h1>

Sesame AI dropped CSM-1B - the billion-parameter engine powering the viral assistant Maya.

This isn't your typical tech release:

- 1 billion parameters

- Hollywood-level realism

- Instant use - zero fine-tuning

- Completely FREE for commercial use

No paywalls. No permissions. Apache 2.0 license.

In simple terms:

Every startup just got handed the keys to Google's and Meta’s top-secret voice tech. 

Just think about it:

→ AI phone reps indistinguishable from humans.

→ Personalized assistants for every creator.

→ Indie devs going head-to-head with ElevenLabs - with zero budget.

Sesame just said:

“Here’s the model. Build whatever you want.”

No APIs. No subscription traps. No corporate gatekeepers.

Voice is the next frontier - and now it's FREE for all.

Fascinating times.

Github Repo: https://github.com/SesameAILabs/csm

Model: https://huggingface.co/sesame/csm-1b

Video credit: Brian Buntz

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/jqHNoTs4Meo?si=M6_GvMtK8CtSvm2B" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

  </div>
</div>

<hr>
<hr>

<h1> DeepSeek AI dropped another 700GB file on Hugging Face with an MIT license. Incredible. </h1>

It casually beats all closed-source players!

They released a new version of their DeepSeek-V3 model, simply called "DeepSeek-V3-0324". It beats all other non-reasoning models, which are models that directly spit out an answer without taking time to ‘think’, making them useful in latency-sensitive use cases. 

They do this at a fraction of the price - the model is priced at $0.27 per 1M input tokens and $1.10 per 1M output tokens, compared to $3 and $15 respectively for Anthropic's API for example.

On the same day, Alibaba's Qwen lab released a 32B VLM which is the best openly available vision-language model out there. It has an Apache 2.0 license which allows for self-hosting.

It is showing once again that Chinese labs choose a different way of releasing things - in an open way, with (upcoming) tech reports. 

Artificial Analysis's thread on this: https://x.com/ArtificialAnlys/status/1904467255083348244

Model: https://huggingface.co/deepseek-ai/DeepSeek-V3-0324

Qwen's 32B VLM: https://huggingface.co/Qwen/Qwen2.5-VL-32B-Instruct

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
   <a href="/assets/img/news/AI news/7.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/7.jpg" 
           alt="Nyx" 
          />
</a>

  </div>
</div>
