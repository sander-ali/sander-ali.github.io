---
layout: page
title: Daily AI news
date: 2025-03-05
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

<h1> 5th March 2025 </h1>

<h1> A2ZRadiology AI just released MC-MED </h1>

We just released MC-MED: 118,385 emergency department visits with continuous physiological waveforms. Nothing like this has existed before.

Our Harvard/Stanford team built what AI Medicine researchers have needed for years—a dataset that captures both the clinical complexity and continuous physiological monitoring of emergency department care.

What's new here:

- Continuous ECG, PPG and respiratory waveforms matched to clinical events

- Complete patient journeys from arrival to disposition

- Pandemic-era data (2020-2022) reflecting modern emergency care

- Scale that enables serious AI applications

This opens up research that was previously impossible—from early detection of deterioration to precision interventions based on physiological patterns.

Built this with an incredible team: Aman Kansal, Emma (Ying) Chen, Tom Jin, and co-PI Prof. David Kim.


Available now on PhysioNet: https://physionet.org/content/mc-med/1.0.0/

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


<h1> Turn any website into LLM-ready data in just a few lines of code! 🔥 </h1>

Introducing Firecrawl an open-source framework that takes a URL, crawls it, and converts it into a clean markdown or structured format.

Key Features:

• 🗂️ Scrape: scrapes a URL and get its content in LLM-ready format (markdown, structured data via LLM Extract , screenshot, html)

• 📑 Crawl: scrapes all the URLs of a web page and return content in LLM-ready format

• ↪️ Map: input a website and get all the website urls - extremely fast

• 🔍 Extract: get structured data from single page, multiple pages or entire websites with AI.

The best part?

It's 100% Open Source


Github Repo: https://github.com/mendableai/firecrawl 

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


<h1>Hugging Face launched LLM Reasoning Course</h1>

HuggingFace has just launched a new free course on "LLM Reasoning" for explaining how to build models like DeepSeek-R1. The course has a special focus towards Reinforcement Learning. The content looks great. Worth giving a try.

Link : https://huggingface.co/reasoning-course


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


<h1> LFGG! Cohere just dropped Aya Vision 32B and 8B </h1>

LFGG! Cohere just dropped Aya Vision 32B and 8B - beats Llama 3.2 90B Vision and Gemini Flash 🔥

> 8B Model: Best-in-class for its parameter size, outperforming competitors by up to 81% win rates 

> 32B Model: Outperforms models 2x its size, achieving 49%-72% win rates

Some notes on the release:

> Supports 23 languages and excelling in tasks like image captioning, visual question answering, and text generation

> Aya Vision 32B outperforms models more than twice its size (e.g., Llama-3.2 90B Vision, Molmo 72B) with win rates of 50%-64% on AyaVisionBench and 52%-72% on mWildVision

> 8B achieves 79%-81% win rates against leading models in its parameter class (e.g., Qwen2.5-VL 7B, Gemini Flash 1.5 8B)

> Uses dynamic resizing and Pixel Shuffle to handle high-resolution images, reducing image tokens by 4x for improved latency and throughput

> Synthetic annotations and translation/rephrasing techniques enhance multilingual data coverage, improving win rates by 17.2% on AyaVisionBench

> Merging vision-language and base language models boosts generative capabilities, increasing win rates by 11.9% on AyaVisionBench

Architecture:

> Vision Encoder: Initialized with SigLIP2-patch14-384 for high-resolution image processing

> Dynamic Resizing: Splits high-res images into tiles, processed with Pixel Shuffle for token compression

> Text Decoder: Initialized from Cohere Command R7B (8B) and Aya Expanse 32B (32B), fine-tuned with multilingual data

> Vision-Language Connector: Aligns image tokens with language model embeddings

Training (Two-Stage Process):

> Vision-Language Alignment: Trains the connector while freezing the vision encoder and LLM

> SFT: Trains both connector and LLM on multilingual multimodal tasks

> Uses synthetic annotations, translation, and rephrasing to expand multilingual coverage

> Model Merging: Combines base LLM with fine-tuned vision-language model to enhance generative performance

Model weights on Hugging Face and integrated on Transformers day-0 🤗


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

<h1> Phi-4 beats SOTA Models </h1>

BOOM! Phi 4 Multimodal (MIT licensed) - the new king of the Open ASR Leaderboard 💥

Beats Nvidia Canary, OpenAI Whisper and more 🤩

Bonus: the model can do much more - speech summarisation, diarization and doubles up as an Audio LM too!

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

<h1> GRPO can do more </h1>

Forget basic math problems. GRPO can do more! If you are exploring Reinforcement Learning you should take a look at the this blog post. 👀

💡 Focuses on ambiguous text judgements (not just clear math answers).

📉 Constant learning rate (1e-6) + warmup beats decaying schedules.

📏 Gradient clipping with max_grad_norm 0.2 keeps training stable (PPO’s secret sauce).

📝 Used XML reward +0.2 reward for perfect formatting only if judgement is correct.

⚡ Explores power-scaling rewards (x⁴) to scale down individual rewards for a overall bad batch.

📏 Tested length based rewards for hitting ~128-tokens.

📈 7B model adapts 3x faster than 3B

🔍 High-reward samples reveal structured reasoning patterns, with phrases like "Both of these..." and "However,"

Read: https://kalomaze.bearblog.dev/grpo-judge-experiments-findings-and-empirical-observations/

Based on: https://github.com/willccbb/verifiers


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

<h1> 🚀 Multimodal RAG with Docling and IBM's Granite 3.2! 🚀 </h1>

We're thrilled to announce a comprehensive tutorial that guides you through building an AI-powered multimodal Retrieval-Augmented Generation (RAG) system using IBM's latest Granite 3.2 model and Docling. 

Why This Matters:

The Granite 3.2 model introduces enhanced reasoning capabilities, enabling more sophisticated understanding and generation of human-like text. When combined with Docling's robust document parsing and conversion features, you can create AI systems that seamlessly process and comprehend diverse data types, including text and images, leading to more accurate and insightful responses.​

Key Highlights:

1. Granite 3.2 Model: Experience the advanced reasoning and multimodal processing capabilities of IBM's latest language model. ​

2. Docling Integration: Efficiently handle and transform documents from various sources using this open-source toolkit. ​

3. LangChain for Workflow Orchestration: Streamline and automate document processing and retrieval workflows, ensuring seamless interaction between different system components.​

This tutorial is ideal for AI developers, researchers, and enthusiasts aiming to deepen their understanding of document management and advanced natural language processing techniques. Embark on this journey to harness the power of multimodal AI and elevate your projects to new heights!​

- tutorial: https://www.ibm.com/think/tutorials/build-multimodal-rag-langchain-with-docling-granite

- github: https://github.com/ibm-granite-community/granite-snack-cookbook/blob/main/recipes/RAG/Granite_Multimodal_RAG.ipynb


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
