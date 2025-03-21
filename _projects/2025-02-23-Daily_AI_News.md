---
layout: page
title: Daily AI news
date: 2025-03-21
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

<h1> 21st March 2025 </h1>

<h1> Every 0.2 seconds on Earth, someone downloads a small language model </h1>

15M times small language models were downloaded from Hugging Face in the last month. How different are these models from each other?

The recent addition to SLM is Gemma-3 (1B to 27B). The new generation of models has a bigger context of 128K tokens. An increased context window size requires more computing and memory. It was solved by Grouped-Query Attention mechanisms and an optimized KV-cache - the model uses 5 local attention layers for 1 global. Gemma-3 is trained on 14T tokens, including text and images. For text data, the model uses the same tokenizer as Gemini 2.0 with a 256K vocabulary size. The SigLIP encoder encodes images. The encoder segments images into non-overlapping crops and uses the P&S method for different aspect ratios. An interesting solution is to keep the image encoder frozen during training; it saves some resources on pre-training of the model, as we can pre-compute embeddings of images. The authors produced different quantized models focusing on open-source inference engines such as llama.cpp.

The Qwen2.5 (0.5B to 72B) model is trained on 18T tokens. It uses GQ attention as Gemma. Vocabulary size is 151K tokens and uses Qwen's tokenizer. Control tokens were expanded from 3 to 22 to support tool-calling functionality and structure output. The model developers use the scaling law to predict future model performance and determine its optimal parameters, such as model size for a given compute budget. In the Qwen paper, it's used for Hyper-parameters, such as batch size and learning rate.

In Dec 2024, the new version of Phi model was released Phi-4 (14B). Phi models are built focusing on quality synthetic data. Every new generation improves the data creation pipeline. The pipeline includes multi-agent prompting, self-revision workflows, and instruction reversal. Additional efforts were spent on preventing data contamination(leaking of benchmarks into training data). The paper describes a hybrid n-gram algorithm that uses 13- and 7-gram features to detect data from benchmarks. The total size of pre-trained data is 10T tokens. The context length of the model is 16K tokens, which is achieved via extending the default context 4K during midtraining. An interesting aspect of the model post-training is the Pivotal Token Search. The idea is based on probabilities that LLM produce during response generation. We can calculate the difference between before and after one token generation. Tokens which impact the overall probability the most are pivotal or crucial decision-making points. So when we do post-training, we should target such pivotal tokens to train the model to make better decisions.

There are more than 70 open-source small language models on the market, and the upper bound of model size is slightly growing. By today's standards, GPT-2 is SLM. However, a few things stay the same: focus on quality data and inference efficiency.


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

<h1> QuantumBlack, AI by McKinsey has released an interesting State of AI in 2025 </h1>

Report packed with interesting statistics. I totally agree with their frame "The value of AI comes from rewiring how companies run." That's the imperative for this year and beyond.

Some of the particularly interesting statistics:

💰 Over half of respondents using generative AI report cost reductions in the business units where it’s deployed.

 📉 More than 80% do not yet see a material enterprise-wide EBIT effect from generative AI, despite functional gains.

 ⚙️ 21% of organizations that have adopted generative AI have fundamentally redesigned some workflows.

 ✅ 71% regularly use generative AI in at least one function, a jump from 65% in early 2024.

 🔎 78% overall use AI in at least one function, up from 55% a year earlier.

 ☑️ 27% review all AI outputs; a similar share checks 20% or less, highlighting wide variation in quality control.

 👤 28% say their CEO oversees AI governance, while 17% name their board of directors.

 ⚠️ Many report mitigating inaccuracy, cybersecurity, and IP risks—cited most often as having caused negative impacts.

 ✍️ 63% of those using generative AI create text, over one-third generate images, and more than one-quarter produce code.

 🔒 13% have hired AI compliance specialists, and 6% have hired AI ethics specialists in the past 12 months.

 🧑‍💻 Fewer respondents call AI hiring “very difficult” compared with previous years, but data scientists remain in high demand.

 🔄 Most organizations have reskilled employees in the past year due to AI; more reskilling is planned over the next three years.

 👥 38% expect little net workforce change from generative AI; service operations and supply chain see the largest reduction risk, while IT and product development may expand.

Full report can be accessed at: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai#/
<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/2.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/2.jpg" 
           alt="Nyx" 
          />
</a>

  </div>
</div>

<hr>
<hr>

<h1>🖲️🖲️Visual Geometry Grounded Transformer🖲️🖲️ </h1>

👉VGGT by VGG & META (CVPR2025) is a feed-forward neural net. that directly infers all key 3D attributes of a scene, including extrinsic/intrinsic cam-params, point maps, depth maps, and 3D point tracks, from one, a few, or hundreds of its views, within seconds. Code released under NC 4.0💙

𝐇𝐢𝐠𝐡𝐥𝐢𝐠𝐡𝐭𝐬:

✅VGGT: Visual Geometry Grounded Transformer

✅Large feed-fwd transformer for 3D attributes

✅Intr/extrinsics, points, depth & 3D point tracks

✅SOTA, better than methods w/ post-processing


👉Paper https://arxiv.org/pdf/2503.11651

👉Project https://vgg-t.github.io/

👉Code https://github.com/facebookresearch/vggt

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

<h1> 🚀 **Mistral Small 3.1: A Game-Changing Open-Source LLM** 🚀 </h1>

Wow! Mistral just dropped a 24B SOTA Multilingual, Multimodal LLM with 128K context AND Apache 2.0 license 🔥

In the fast-paced world of AI, Mistral has released **Mistral Small 3.1**, a powerful open-source model that outperforms many industry leaders. At 24B parameters, it runs efficiently on an RTX 4090 or a Mac with 32GB RAM, making it a lightweight yet robust solution for developers and enthusiasts.

💡 **Key Features:**

✅ **Multimodal & Multilingual:** Seamlessly handles text, images, and 21+ languages.

✅ **Fast & Efficient:** Processes 150 tokens per second with a 128K context window.

✅ **Apache 2.0 License:** Fully open-source for use, fine-tuning, and integration.

📊 **Performance:**

Mistral Small 3.1 excels in:

- **Math & Logical Reasoning**

- **Programming & Code Generation**

- **Multimodal Image Understanding**

- **Long-Context Retention**

Ideal for AI applications, multimodal projects, or local AI setups, this model stands out in the open-source AI landscape.

HF Access: https://huggingface.co/mistralai/Mistral-Small-3.1-24B-Instruct-2503


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

<hr>
<hr>

<h1> Hugging Face just dropped SmolDocling </h1>

🚀 We just dropped 𝗦𝗺𝗼𝗹𝗗𝗼𝗰𝗹𝗶𝗻𝗴: a 𝟮𝟱𝟲𝗠 𝗼𝗽𝗲𝗻-𝘀𝗼𝘂𝗿𝗰𝗲 𝘃𝗶𝘀𝗶𝗼𝗻 𝗟𝗠 for complete document OCR! ✨

📄 𝗘𝗻𝗱-𝘁𝗼-𝗲𝗻𝗱 𝗱𝗼𝗰𝘂𝗺𝗲𝗻𝘁 𝗰𝗼𝗻𝘃𝗲𝗿𝘀𝗶𝗼𝗻—no more complex pipelines, just one tiny model

⚡ 𝗙𝗮𝘀𝘁 & 𝗹𝗶𝗴𝗵𝘁𝘄𝗲𝗶𝗴𝗵𝘁—processes a page in 0.35 sec on a consumer GPU with <500MB VRAM

🏆 𝗦𝗢𝗧𝗔 𝗮𝗰𝗰𝘂𝗿𝗮𝗰𝘆—outperforms models 27× larger in full-page transcription, layout detection, and code recognition

💾 Efficient large-batch processing—cheap and easy to run in-house

📊 Handles all document elements—tables, charts, code, equations, lists, and more

🔍 Full tech report available with release

This is another example that small, optimized models can compete with much larger systems—making AI more sustainable.

Model: https://huggingface.co/ds4sd/SmolDocling-256M-preview

Paper: https://arxiv.org/abs/2503.11576

Code: https://github.com/docling-project/docling

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/7oi5H9M4gfE?si=NXcIkGvE1BKWCVjB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


  </div>
</div>

<hr>
<hr>

<h1> New RL Method thats better than GRPO!  </h1>

New RL Method thats better than GRPO! 🤯 ByteDance released a new open source RL method that outperforms GRPO 👀 DAPO or Decoupled Clip and Dynamic sAmpling Policy Optimization (DAPO) achieves 50 points on the AIME 2024 with 50% fewer training steps.

TL;DR: 

🏆 50% AIME 2024 accuracy (Qwen2.5-32B), surpassing DeepSeek-R1 with 50% fewer steps.

🤗 Fully open-source: code (based on verl), training dataset (DAPO-Math-17k), and model weights (soon)

💡 Clip-Higher: Asymmetric clipping bounds with higher upper bound to prevent entropy collapse

🔄 Dynamic Sampling: Filters out prompts with 0% or 100% accuracy

🔍 Token-level Policy Gradient Loss: Prevents excessive response lengths and maintains reasoning quality

📏 Length-aware penalty: Reduce reward noise for truncated, but potentially valid, long responses.

✅ Uses simple, robust rule-based verifier based on string normalization and matching

🛠️ Compared to GRPO: No KL divergence penalty, token-level loss (vs sample-level), asymmetric clip ranges and filtering.

🥇Qwen2.5-32B DAPO achieves 50 points on AIME vs. GRPO's 30 points

⚠️ Release excludes Dynamic Sampling in scripts (44% AIME)

project page: https://dapo-sia.github.io/

code: https://github.com/BytedTsinghua-SIA/DAPO

paper: https://huggingface.co/papers/2503.14476

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

<hr>
<hr>

<h1> Robots finally got real! </h1>

Jensen Huang just introduced Blue (Star Wars droid) and NVIDIA's partnership with DeepMind and Disney 👏🥹

At Nvidia's GTC 2025, CEO Jensen Huang introduced a droid straight out of your Star Wars dreams 🤖

Blue isn't just a prop - it's an interactive droid designed to:

- Walk and move fluidly.

- Engage naturally with humans.

- Bring Star Wars to life, right before your eyes.

To achieve that, three giants joined forces:

↳ NVIDIA’s expertise in AI and computing.

↳ Google DeepMind’s advancements in machine learning.

↳ Disney’s creative storytelling.

They're also launching Newton, an open-source physics engine. It's a digital playground where robots learn real-world skills through lifelike simulations.

The future is here, and it's amazing.

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
   <iframe width="560" height="315" src="https://www.youtube.com/embed/YxH4Mx6zh6c?si=CwG8J81JEBNGxOae" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

  </div>
</div>
