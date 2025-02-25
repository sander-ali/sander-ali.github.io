---
layout: page
title: Daily AI news
date: 2025-02-24
description: This page is dedicated to your daily AI news especially related to Agents, LLMs, and Agentic AI
img: assets/img/news/logo_SAK_15.PNG

images:
  lightbox2: false
  photoswipe: true
  spotlight: false
  venobox: false
---


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/logo_SAK_15.PNG"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/logo_SAK_15.PNG" 
           alt="Comapny Logo" 
           style="width: 1200px; height: 800px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>

<h1> 25th February 2025 </h1>

<h1> News 1 </h1>

DeepSeek released their first open-source repo for this week! FlashMLA uses CUDA kernels to make hosting DeepSeek AI's R1 + V3 faster! Optimized multi latent attention CUDA kernels - currently BF16 for now and maybe FP8 in the future?


They'll be releasing 4 (or more) packages per day for remainder of this week!


Github package: https://github.com/deepseek-ai/FlashMLA

To understand MLA (multi-head latent attention) better,

see https://www.linkedin.com/posts/danielhanchen_deepseek-v3-is-the-most-powerful-open-source-activity-7278488573006200832-KtA_/

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/1.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/1.jpg" 
           alt="Byte Dance" 
           style="width: 640px; height: 480px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>

<h1> News 2 </h1>

LLMs “think harder” in a latent space? New paper demonstrates that by allowing LLMs to iterate in its latent space (like "thinking" multiple times about the same input) improves performance comparable to much larger models.

Implementation (simplified):

1️⃣ 3-part architecture: 1. Prelude: Transforms input tokens into latent space; Recurrent Block: Core "thinking" component that iterates multiple times; Coda: Converts final latent state to output tokens

2️⃣ Train with randomized recurrence steps (log-normal Poisson sampling) and truncated backpropagation through last 8 iterations

3️⃣ Deploy with dynamic recurrence steps (4-64) at inference for compute scaling with KV-cache sharing and KL-based early stopping for efficiency.

Insights:

📈 Achieves 34.8% strict accuracy on GSM8K (5x baseline) with 32 recurrence
🛠️ "Sandwich" normalization and input reinjection prevent hidden state collapse

📚 Performs best on code/math tasks (23% HumanEval) with data mix containing 31.5% STEM content

🔄 Shows latent space "reasoning orbits" that correlate with task difficulty

⚡ KV-cache sharing reduces memory usage by 75% during long reasoning chains

📚 Performance gains vary by task; easier tasks saturate with fewer iterations, while harder tasks benefit from more.

Paper: https://huggingface.co/papers/2502.05171

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/2.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/2.jpg" 
           alt="Google Gemini 2.0" 
           style="width: 800px; height: 800px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>


<h1> News 3 (Story from Swan AI </h1>

Bolt and Lovable just went from zero to $15M ARR in 2 months with 15 employees. Media calls them "AI miracles". Yet everyone missed the real story: We're witnessing the first wave of autonomous businesses in history.

While the TechCrunch headlines are obsessing over their AI, that's not what makes them special.

These companies aren't winning because of their AI. They're winning because they've cracked a completely new operating system for building companies.

The math tells the story:

Traditional SaaS: $150K-250K revenue per employee

Autonomous businesses: $2M-3M+ per employee

And the spoiler: It's not about replacing humans with AI agents. 

It's about turning your existing talent into superhumans - empowering a small team to operate at enterprise scale.

These companies didn't automate their humans away.

They fundamentally reimagined how humans and AI work together.

Where traditional companies build armies of specialists, autonomous businesses build small teams of strategic orchestrators.

They're proving that the old playbook is dying:

Hire 50+ engineers to "figure out" what to build

Build a 100-person sales team to brute force growth

Burn $2M+ on ads hoping to find what works

Here's what the autonomous playbook actually looks like:

Demand Engine:

- AI: Qualifying 1000s of leads in real-time

- Humans: Small team of strategists owning $100K+ opportunities

- Result: 3-person team >> 50-person sales org

Product Development:

- AI: Handling 80% of code execution

- Humans: Product leaders owning vision & strategy

- Result: 5 builders shipping faster than 50 engineers

Customer Success:

- AI: Managing 90% of support queries

- Humans: Strategic CSMs crafting expansion plays

- Result: 2 humans driving same NRR as 20-person teams

The pattern becomes clear:

While traditional companies spread themselves thin, autonomous businesses concentrate human firepower where it matters most.

At Swan AI, we're not just talking about this future - we're building it:

3 founders

$0 spent on ads

30+ AI agents

And a goal to hit $30M ARR without hiring a single employee.

Because building an autonomous business isn't about replacing humans.

It's about empowering small teams to achieve impossible scale.

The era of bloated teams is over.

The age of the autonomous business has begun.

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/3.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/3.jpg" 
           alt="Google Gemini 2.0" 
           style="width: 800px; height: 800px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>


<h1> News 4 </h1>

🚀 Microsoft Prepares for GPT-5: The AI Evolution Continues

Big moves in AI! Microsoft is gearing up to host OpenAI’s latest models, with GPT-4.5 expected next week and GPT-5 projected for late May. Here’s what’s coming:

🔹 GPT-4.5 (Orion): Faster, more powerful—OpenAI’s final model before a major shift.

🔹 GPT-5: Featuring OpenAI’s o3 reasoning model, setting a new standard for intelligence.

🔹 Smarter ChatGPT: Expect a seamless AI experience with fewer model-switching headaches.

🔹 Microsoft’s Play: Watch for Copilot updates and AI breakthroughs at Build 2025.

AI is evolving fast—how do you see GPT-5 shaping the future?

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/4.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/4.jpg" 
           alt="Google Gemini 2.0" 
           style="width: 800px; height: 800px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>

<h1> News 5 from Anthropic </h1>

Anthropic Introduces Claude 3.7 Sonnet: their most intelligent model to date. It's a hybrid reasoning model, producing near-instant responses or extended, step-by-step thinking. One model, two ways to think.

Claude 3.7 Sonnet is a significant upgrade over its predecessor. In extended thinking mode, it self-reflects before answering, which improves its performance on math, physics, instruction-following, coding, and many other tasks.

We generally find that prompting for the model works similarly in both modes. API users also have fine-grained control over how long the model can think for.

Claude 3.7 Sonnet is a state-of-the-art model for coding and agentic tool use. However, in developing it, we optimized less for math and computer science competition problems, and more for real-world tasks. We believe this more closely reflects the needs of our customers.

We conducted extensive model testing for safety, security, and reliability. We also listened to your feedback. With Claude 3.7 Sonnet, we've reduced unnecessary refusals of requests by 45% compared to its predecessor.

Claude 3.7 Sonnet and Claude Code mark an important step towards AI systems that can truly augment human capabilities.

We look forward to seeing what you'll create. And we welcome your feedback as we continue to build. https://www.anthropic.com/news/claude-3-7-sonnet

<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/5.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/5.jpg" 
           alt="Google Gemini 2.0" 
           style="width: 640px; height: 480px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>

<h1> News 6 </h1>

New Agent/Function Calling Leaderboard from Galileo evaluates 17 LLMs across 14 benchmarks. Foundation models like Google DeepMind Gemini-2.0-flash and OpenAI GPT-4o lead, but open models are catching up. 👀

🎯 Evaluates single-turn, multi-turn, error handling, and context management using Tool Selection Quality (TSQ)

🎲 TSQ measures if models choose the right tools, use correct parameters, and know when NOT to use tools at all, evaluated with LLM as a Judge

📊 Uses datasets from BFCL, τ-bench, xLAM, and ToolACE covering 400+ domains

🏆 Gemini-2.0-flash leads the pack with 0.938 score, followed by GPT-4o at 0.900

🚀 Open models are catching up - mistral-small-2501 achieves 0.832

🚫 Some models like DeepSeek excluded due to limited function calling support

📌 Monthly updates planned to keep pace with new model releases

Leaderboard: https://huggingface.co/spaces/galileo-ai/agent-leaderboard

Blog: https://www.galileo.ai/blog/agent-leaderboard


<div style="display: flex; justify-content: center; align-items: center;">
  <div class="pswp-gallery pswp-gallery--single-column" id="gallery--news" style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
    <a href="/assets/img/news/AI news/6.jpg"
      data-pswp-width="1200" 
      data-pswp-height="800"
      target="_blank">
      <img src="/assets/img/news/AI news/6.jpg" 
           alt="Google Gemini 2.0" 
           style="width: 640px; height: 480px; object-fit: cover; border-radius: 8px;" />
</a>

  </div>
</div>

<h1> News 7 </h1>
Artificial intelligence (AI)-powered search engine Perplexity AI is planning on launching its own web browser.

The company said in a post on X on Monday (Feb. 24) that the browser, dubbed Comet, was “coming soon,” and invited people to sign up on a waitlist in a reply.

“Just like Perplexity reinvented search, we’re also reinventing the browser,” a Perplexity spokesperson told TechCrunch via email, the publication reported on Monday. “Stay tuned for updates.”

The company said in October that its search engine served over 100 million queries per week.

“Perplexity now serves over 100M queries every week,” Perplexity CEO Aravind Srinivas wrote in a post on X at the time. “Next stop: 100M+ queries every day.”

In December, Perplexity reportedly closed a $500 million funding round, tripling the startup’s valuation to $9 billion, according to a PYMNTS rerpot. The company’s backers included SoftBank, Nvidia and Amazon founder Jeff Bezos, according to the report. Perplexity had a valuation of $520 million early in 2024. During that summer, it was valued at $3 billion.

In November, the company introduced an AI-powered shopping assistant for U.S. consumers.

Through Buy With Pro, shoppers can research and purchase products, Perplexity said in a Nov. 18 blog post.

“It marks a big leap forward in how we serve our users — empowering seamless native actions right from an answer,” the company said in the post. “Shopping online just got 10x more easy and fun.”

The feature is only available to Perplexity Pro users in the U.S. It lets users check out on the company’s website or app for select products from select merchants, according to the post. Consumers who save their shipping and billing information on the portal can use a one-click checkout option.

Additionally, Perplexity unveiled a visual search tool called Snap to Shop, which helps consumers find an item by uploading a photo. Snap to Shop will display relevant products based on the photo, with no need for a product description or name, according to the post.

In other search engine news, a recent Bank of America Global Research report found that global daily visits to Google search are “stable” despite the surge in the number of artificial intelligence (AI)-powered chatbots like ChatGPT, Perplexity and Claude.

In January, the global average daily visits to Google were up 1% to 2.7 billion from December and down just 1% year over year, according to the report. The daily visits include desktop and mobile searches.

Google’s continued search engine dominance comes as AI chatbots continue to grow in popularity. Last month, visits to ChatGPT were up 4% month over month and 148% year over year to 128 million globally.

source: https://www.pymnts.com/artificial-intelligence-2/2025/ntt-data-cdao-c-suite-leaders-have-angst-about-genai-still-go-full-throttle/