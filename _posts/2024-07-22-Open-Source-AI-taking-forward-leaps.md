---
layout: post
title: Open Source AI taking forward leaps
date: 2024-07-22 09:00:00-0400
tags: [Open Source AI, LLM, Mistral AI, Apple AI, Salesforce]
thumbnail: assets/img/blog/Open_models_1.png
---


Most progressive week in the history of Open Source AI (yet):

1. Mistral (in collaboration with Nvidia) dropped Apache 2.0 licensed NeMo 12B LLM, better than L3 8B and Gemma 2 9B. Models are multilingual with 128K context and a highly efficient tokenizer — tekken.

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_1.png" class="img-fluid rounded z-depth-1" %}

2. Apple released DCLM 7B — truly open source LLM, based on OpenELM, trained on 2.5T tokens with 63.72 MMLU (better than Mistral 7B)

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_2.png" class="img-fluid rounded z-depth-1" %}

3. HF shared SmolLM — 135M, 360M, & 1.7B Smol LMs capable of running directly in the browser; they beat Qwen 1.5B, Phi 1.5B and more. Trained on just 650B tokens.

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_3.png" class="img-fluid rounded z-depth-1" %}

4. Groq put out Llama 3 8B & 70B tool use & function calling model checkpoints — achieves 90.76% accuracy on Berkely Function Calling Leaderboard (BFCL). Excels at API usage & structured data manipulation!

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_4.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_5.png" class="img-fluid rounded z-depth-1" %}

5. Salesforce released xLAM 1.35B & 7B Large Action Models along with 60K instruction fine-tuning dataset. The 7B model scores 88.24% on BFCL & 2B 78.94%

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_6.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_7.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_8.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_9.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_10.png" class="img-fluid rounded z-depth-1" %}

6. Deepseek changed the game with v2 chat 0628 — The best open LLM on LYMSYS arena right now — 236B parameter model with 21B active parameters. It also excels at coding (rank #3) and arena hard problems (rank #3)

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_11.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_12.png" class="img-fluid rounded z-depth-1" %}

{% include figure.liquid loading="eager" path="assets/img/blog/Open_models_13.png" class="img-fluid rounded z-depth-1" %}

There’s a lot more; Arcee (mergekit) released a series of LLMs, each better than the other, and Numina and HF Numina 72B (based on Qwen 2) and Math datasets, Mixbread with embedding models (english + german) and a lot more!
