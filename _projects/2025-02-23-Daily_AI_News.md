---
layout: page
title: Daily AI news
date: 2025-03-13
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

<h1> 13th March 2025 </h1>

<h1> Reka Flash 3: a 21B reasoning model with great performance </h1>

Reka recently open-sourced a preliminary version of Reka Flash 3, a 21 billion parameter multimodal language model designed to excel at tasks like general chat, encoding, instruction, and function calls. This compact model offers competitive performance compared to proprietary solutions like OpenAI o1-mini, making it ideal for applications that require low latency or local device deployments. Its ability to handle contexts of up to 32,000 tokens makes it particularly versatile.

Key Points:

- 21 billion parameter open source model

- Competitive performance with proprietary solutions

- Support for extended contexts of up to 32,000 tokens

- Suitable for low latency and local device applications

Reka Flash 3’s training process was meticulous, starting with pre-training on a heterogeneous set of synthetic and publicly accessible data. Next, the model was tuned with instructions based on high-quality, curated data to improve its performance. In the final step, reinforcement learning was applied using REINFORCE Leave One-Out (RLOO), leveraging both model-based and rule-based rewards to further enhance its capabilities. Unlike models that specialize in mathematics or coding, Reka Flash 3 aims for general improvements through reinforcement learning.

Reka Flash 3’s performance is remarkable: on AIME-2024, with a budget of 16 reasoning steps, the model demonstrated significant efficiency. Additionally, on WMT’23, it achieved a COMET score of 83.2, showing improvements over previous versions in multilingual understanding. However, as a more compact model, it may not be the ideal option for tasks that require extensive knowledge, as indicated by its MMLU-Pro score of 65.0. Therefore, it is recommended to integrate it with web search for tasks that require in-depth knowledge.

A distinctive aspect of Reka Flash 3 is its ability to "think" before generating an answer, using tags to delimit the reasoning process. This mechanism allows the model to stop reasoning after a certain number of steps, while still ensuring reasonable outputs. This feature allows processing time to be managed according to predefined budgets, providing flexibility to developers.

In terms of deployment, Reka Flash 3 is optimized for low-cost applications that require low latency or execution on local devices. At full precision, the model occupies 39 GB (fp16), but can be compressed up to 11 GB while maintaining high performance thanks to 4-bit quantization. This makes it more efficient than larger models such as the QwQ-32B, which requires 64 GB at bf16 and 18 GB with 4-bit quantization.

It is important to note that while Reka Flash 3 was designed primarily for English, it has demonstrated some understanding of other languages. However, in some cases, the model may process English reasoning even when questions are asked in other languages, impacting the quality of the output. Additionally, the model has not undergone extensive alignment or training, suggesting room for improvement in the future.

For those who want to test Reka Flash 3, a trial version is available on Reka Space. Additionally, the model weights are downloadable and modifiable under the Apache 2.0 license, providing developers and researchers with a powerful yet lightweight foundation on which to build custom applications. 

Reka Flash 3 represents a significant step forward in the field of multimodal language models, combining efficiency, versatility, and accessibility, opening up new opportunities for innovative applications in the AI ​​field.

Source: https://www.turtlesai.com/en/pages-2470/reka-flash-3-a-21b-reasoning-model-with-great 

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


<h1> 🦜🪞LangGraph-Reflection </h1>

This prebuilt graph is an agent that uses a reflection-style architecture to check and improve an initial agent's output.

This reflection agent uses two subagents:

- A "main" agent, which is the agent attempting to solve the users task

- A "critique" agent, which checks the main agents work and offers any critiques

`pip install langgraph-reflection`

YouTube video: https://www.youtube.com/watch?v=rBWrjNyVyCA

GitHub: https://github.com/langchain-ai/langgraph-reflection



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


<h1>OpenAI just released Agents SDK for building multi-agent apps in Python 🤯 </h1>

OpenAI just launched their official agents framework - if you’re an AI agent developer or builder, here’s everything you need to know (coming from a founder building their own agents platform):

=> What is it?

OpenAI “Agents SDK” is an open source agents framework with a core abstraction of agents + handoffs. For example: user sends a message “Hola, como estas?”, which gets sent to a “triage agent”, which then routes the request to the “Spanish agent” instead of the “English agent”.

=> Is OpenAI “Agents SDK” open source and model-agnostic?

“Agents SDK” is open source and can be configured to work with third parties that support the ChatCompletions API.

However - OpenAI’s new agent tracing is not open source. To use tracing, you have to log into OpenAI’s website and view their tracing dashboard.

Remind anyone of LangChain (OSS) + LangSmith (closed source / SaaS product)?

Additionally, OpenAI recommends users of the “Agents SDK” use their new Response API (which stores message histories, similar to the Assistants API). Currently, OpenAI is the only provider that supports this API.

=> What does this mean for other agent frameworks?

Direct competition from the model providers. As the model layer commoditizes, OpenAI is starting to make plays in the framework layer.

=> What’s the difference between OpenAI’s agents framework and other open source agents frameworks?

Forced “Handoff” abstraction: Like all abstractions, useful for some use-cases, and not a great fit for others.

State is a second-class citizen: Similar to most agents frameworks, memory and state are not first party concepts - agents in OpenAI's Agents SDK do not have built-in support for long-term memory or context management. It’s expected that you run your agent script once, then “throw it away” - similar to a workflow.

=> What’s next for OpenAI?

It makes complete sense for OpenAI to be moving up the agents stack as the model layer commoditizes - "Agents SDK" is just an initial step.

My take: OpenAI's end-game (on the developer side) is a fully hosted stateful agents service, similar to their Custom GPTs or Assistants API. I expect to see a revised version of the Assistants API launch soon, likely rebranded as an “Agents API” (a paid hosted service that can integrate with the open source “Agents SDK”).

=> Why will / won’t OpenAI win?

The problem for OpenAI is that developers do not want model or data lock-in in their agents stack.

Developers want to be able to move their agent state (messages, tools, user data, data sources, memories) across model providers with zero friction. This is why provider-agnostic frameworks will win out over first party options made by OpenAI (or other frontier labs).

Imagine if you built a verticalized agent startup on the OpenAI Assistants API in 2024. Your entire app is locked into OpenAI with no escape - no Sonnet, no DeepSeek V3/R1.

The rise of stateful agents (e.g. agents with long-term memory) makes model lock-in even more devastating.

- More commentary on what makes up the "agents stack": https://www.letta.com/blog/ai-agents-stack

- The official OpenAI Agents SDK documentation: https://openai.github.io/openai-agents-python/ 

- The new Responses API spec: https://platform.openai.com/docs/api-reference/responses/create



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


<h1> AI Innovation in Europe </h1>

Today the EuroHPC Joint Undertaking (EuroHPC JU) has selected six additional proposals to establish AI Factories in the EU powered by EU’s world-class network of supercomputers.
 
The newly selected AI Factories will be hosted in Austria, Bulgaria, France, Germany, Poland and Slovenia, supported by a combined national and EU investment of around €485 million.
 
Together with the first selection of seven AI Factories, they will bring the key ingredients for AI innovation: computing power, data and talent, fully unlocking the potential of AI in Europe.
 
The factories will enable AI companies, in particular SMEs and startups, as well as researchers, to enhance the training and development of large-scale trustworthy and ethical AI models.
 
Find out more information: https://europa.eu/!F6KGPG

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

<h1> Google is BACK!! Welcome Gemma3  </h1>

Google is BACK!! Welcome Gemma3 - 27B, 12B, 4B & 1B - 128K context, multimodal AND multilingual! 🔥

Gemma 3 is here and its the best open non-reasoning model on LMSYS! 🚀Google DeepMind Gemma 3 is an open, multimodal (text + vision), multilingual LLM with a context of 128k tokens and comes in 4 sizes!

Evals:

> On MMLU-Pro, Gemma 3-27B-IT scores 67.5, close to Gemini 1.5 Pro (75.8)

> Gemma 3-27B-IT achieves an Elo score of 133 in the Chatbot Arena, outperforming larger LLaMA 3 405B (1257) and Qwen2.5-70B (1257) 

> Gemma 3-4B-IT is competitive with Gemma 2-27B-IT 🤯

Multimodal:

> Vision understanding via a tailored SigLIP vision encoder, treating images as sequences of soft tokens

> Pan & Scan (P&S): An adaptive windowing algorithm segments non-square images into 896x896 crops, improving perf in high-resolution images

Long Context:

> Supports up to 128K tokens (except for the 1B model, which supports 32K)

> Uses a 5:1 ratio of local to global attention layers to reduce KV-cache memory explosion 

> Local layers have a span of 1024 tokens, while global layers handle long context

Memory Efficiency:

> The 5:1 local-to-global attention ratio reduces KV-cache memory overhead from 60% (global-only) to less than 15%

> Quantization Aware Training (QAT) is used to provide models in int4, int4 (per-block), and switched fp8 formats, significantly reducing memory footprint

Training and Distillation:

> Pre-trained on 14T tokens for the 27B model, with increased multilingual data

> Uses knowledge distillation with 256 logits per token, weighted by teacher probabilities

> Post-training focuses on improving math, reasoning, and multilingual abilities, with a novel approach that outperforms Gemma 2

Vision Encoder Performance:

> Higher resolution encoders (896x896) outperform lower resolutions (256x256) on tasks like DocVQA (59.8 vs. 31.9)

> P&S boosts performance on tasks involving text recognition, e.g., DocVQA improves by +8.2 points for the 4B model

Long Context Scaling:

> Models are pre-trained on 32K sequences and scaled to 128K using RoPE rescaling with a factor of 8

> Performance degrades rapidly beyond 128K tokens, but models generalise well within this limit

Try in AI Studio: https://aistudio.google.com/prompts/new_chat?model=gemma-3-27b-it

Models: https://huggingface.co/collections/google/gemma-3-release-67c6c6f89c4f76621268bb6d

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

<h1> Olympic Coder </h1>

Announcement by Hugging Face

We've kept pushing our Open-R1 project, an open initiative to replicate and extend the techniques behind DeepSeek-R1.

And even we were mind-blown by the results we got with this latest model we're releasing: ⚡️OlympicCoder

It's beating Claude 3.7 on (competitive) programming –a domain Anthropic has been historically really strong at– and it's getting close to o1-mini/R1 on olympiad level coding with just 7B parameters!

And the best part is that we're open-sourcing all about its training dataset, the new IOI benchmark, and more in our Open-R1 progress report #3: https://huggingface.co/blog/open-r1/update-3

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

<h1> 🤖 Can AI Truly Capture Emotion? OpenAI’s Latest Model Might </h1>

Sam Altman says OpenAI’s newest AI model did something unexpected—it moved him.

When prompted to write about AI and grief, the model’s response wasn’t just well-crafted; it was deeply resonant. According to Altman, this is the first time AI-generated writing has genuinely made him pause.

🔸The story explored themes of loss, memory, and the fine line between imitation and true emotion.

🔸The model shows a striking grasp of metafiction and human sentiment.

🔸OpenAI hasn’t yet shared when (or if) this model will be released.

As AI storytelling evolves, the big question remains: Can it ever go beyond simulation and truly feel?

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
