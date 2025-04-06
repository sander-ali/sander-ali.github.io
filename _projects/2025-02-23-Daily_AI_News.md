---
layout: page
title: Daily AI news
date: 2025-04-07
description: This page is dedicated to your daily AI news especially related to Agents, LLMs, and Agentic AI
img: assets/img/news/logo_SAK_15.PNG

images:
  lightbox2: false
  photoswipe: false
  spotlight: false
  venobox: false
---

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/logo_SAK_15.PNG"
      target="_blank">
      <img src="/assets/img/news/logo_SAK_15.PNG" 
           alt="Comapny Logo" 
           />
</a>
    
  </div>
</div>

<h1> 7th April 2025 </h1>

<hr>
<hr>

<h1> Dream 7B is a powerhouse Diffusion reasoning model, streaming its responses like a pro 👇  </h1>

Unlike AR models, which generate text sequentially (left-to-right), Dream 7B enables any-order generation, unlocking new possibilities for solving complex reasoning tasks, long-term planning, and maintaining coherence across extended contexts. Its innovative context-adaptive token-level noise rescheduling mechanism ensures precise learning at the token level, setting a new benchmark in LLM training.

✨ Key Highlights of Dream 7B:

• Advanced Reasoning Capabilities: Outperforms similar-sized AR models in tasks like Sudoku and Countdown, even rivaling larger models like DeepSeek V3.

• Flexible Inference: Supports diverse user queries by dynamically adjusting decoding behavior and generation order.

• Efficiency at Scale: Reduces computational requirements during pretraining while offering a tunable trade-off between speed and quality during inference.

• Real-World Applications: Excels in general, mathematical, and coding tasks, with a special focus on solving problems with multiple constraints.

The Github repository can be accessed <a href="https://github.com/HKUNLP/Dream">here</a>

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
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

<h1> Chunking in RAG </h1>

In RAG, "chunking" refers to the process of dividing large documents into smaller, manageable segments called "chunks," which allows the AI model to more efficiently search and retrieve relevant information by focusing on smaller, contextually cohesive pieces of text instead of processing the entire document at once; essentially, it breaks down complex information into easily digestible units for better understanding and response generation. 

How chunking works in RAG:

- Dividing text:

Documents are split into chunks based on various strategies, including splitting at paragraph breaks, sentence boundaries, or even using semantic analysis to identify logical topic shifts within the text. 

- Embedding creation:

Each chunk is then converted into a vector embedding, which represents the semantic meaning of the text within that chunk. 

- Query comparison:

When a user asks a question, the query is also transformed into a vector embedding and compared to the embeddings of all the chunks in the document database. 

- Relevance ranking:

The system identifies the chunks with the highest similarity to the query, meaning they are most likely to contain the relevant information. 

- Response generation:

The retrieved chunks are then used by the language model to generate a comprehensive response to the query, drawing from the most relevant information across the selected chunks. 


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
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

<h1>  DeepSeek strikes again!  </h1>

A new DeepSeek AI paper reveals how smaller models can surprisingly outperform giants through clever inference techniques rather than parameter scaling. 

Reward models are the unsung heroes behind AI alignment, providing critical feedback signals that guide LLMs toward producing high-quality, human-aligned responses. 

As these systems grow increasingly complex, the traditional approach of simply scaling up model size to improve performance has become prohibitively expensive and inefficient. 

Self-Principled Critique Tuning (SPCT) is a new method that enables generative reward models to adaptively formulate principles and critiques based on input queries. 

Rather than investing in larger models, they focus on inference-time scaling through parallel sampling and meta-reward modeling. 

With success: their 27B parameter model outperforms alternatives up to 671B parameters on standard benchmarks. 

They demonstrate that thoughtful sampling strategies can effectively substitute for raw parameter count, challenging the conventional wisdom that bigger always means better in AI development. 

Information Courtesy: LLM Watch and Pascal Biese


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

<h1> OpenAI just launched their Academy.  </h1>

We just built something fun with Hugging Face’s new tool— An AI crossword puzzle 🧩 

Free AI courses are here: 

You can access hours of content today.

This includes video, workshops, and live sessions. 

Anyone with an email and LinkedIn can join. 

The curriculum covers all skill levels. 

It starts with basic AI concepts. 

It goes deep into advanced techniques. 

Special topics like AI safety & ethics are included. 

Credits to The AI Radar for sharing it.

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

<h1>  🚨 Big news: Langflow Desktop is HERE! 🚀 </h1>

No browser. No setup. No distractions. Just pure, local GenAI building power.

💻 Langflow Desktop (Alpha) is now available for MacOS

Why this is very exciting:

1/ Instant setup – No Python installs or environment configs.

2/ Runs locally – Full control, zero friction.

3/ Built for builders – Test and iterate faster than ever.

Langflow is all about making it effortless to build and ship AI agents.

Thanks for Armand Ruiz for sharing it.


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

<h1> Midjourney Surprise Launches V7 Alpha 🚀  </h1>

Key features:

🔹Enhanced Image Quality: V7 boasts improved textures, coherence in details, and superior handling of text and image prompts.

🔹Personalization by Default: Users can create a tailored profile in just 5 minutes, enabling outputs that align with their unique preferences.

🔹Draft Mode for Speed: Generate images 10x faster at half the cost, perfect for rapid ideation and real-time adjustments.

🔹Two Modes Available: Turbo mode for speed enthusiasts and Relax mode for optimized workflows.

What excites you most about V7’s capabilities?


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/6.jpg"

      target="_blank">
      <img src="/assets/img/news/AI news/6.jpg" 
           alt="Nyx" 
          />
</a>


  </div>
</div>

<hr>
<hr>

<h1> 🔬 OpenAI's PaperBench: Testing AI's Ability to Replicate Research Papers </h1>

Ever wondered if AI could replicate its own research? OpenAI just dropped PaperBench, and it's giving us a glimpse into our AI future.

Imagine dropping an AI into a virtual machine with nothing but a research paper and telling it: "Build this from scratch." That's PaperBench in a nutshell.

🧠 What caught my attention:

These AI agents must:

- Decode complex research papers 📝

- Write code without any templates 💻

- Debug their own work 🔍

- Reproduce exact results 📊

All while locked in a VM with a GPU and zero human hand-holding!

🏆 Current standings:

Claude 3.5 Sonnet leads with 21% overall (impressive!)

OpenAI's o1 follows at 13-24%

Human ML PhDs still dominate at 41.4%

But here's what's fascinating - the latest powerhouses haven't even entered the arena yet: O3 pro high, Claude 3.7 Sonnet, Gemini 2.5 Pro, and Grok 3 remain untested.

🚀 Why this keeps me up at night:

If models master this benchmark, we're looking at potential recursive self-improvement loops. AI that can understand, replicate, and potentially improve upon AI research without humans in the loop. That can even lead to the Sci-fi esque Artificial Super intelligence.

The implications? Mind-blowing acceleration of progress. AI becoming its own researcher, developer, and innovator.

We're not there yet - current models excel at writing code but stumble when executing it or verifying results. But make no mistake, the race is on.

What do you think? Are we witnessing the early days of AI taking the reins of its own evolution? The age of ASI is surely within my lifetime. I can feel it.

Post Credit: Kishore Kumar

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
