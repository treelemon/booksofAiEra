# Chapter 3: From GPT to Reasoning Models

## 3.1 The GPT Lineage

The GPT family is not just a product line — it is the closest thing AI has to a family tree. Each generation revealed something unexpected about what happens when you scale a decoder-only transformer.

**GPT-1 (June 2018, 117M parameters):** A proof of concept. OpenAI showed that generative pre-training followed by fine-tuning could outperform task-specific architectures. Few noticed.

**GPT-2 (February 2019, 1.5B parameters):** The controversy that woke the world. The generated text was coherent enough that OpenAI, fearing misuse, initially refused to release the full model. The decision sparked a furious debate about responsible disclosure. When the full model finally emerged months later, the community understood for the first time: scale was not just engineering — it was capability.

**GPT-3 (May 2020, 175B parameters, $4.6M training cost):** The earthquake. 175 billion parameters trained on ~570GB of text. The cost was staggering: an estimated $4.6 million for a single training run. But the result was something nobody predicted — **in-context learning**. Without any gradient updates, GPT-3 could perform tasks simply by seeing examples in the prompt. Translate English to French. Write Python from a comment. Answer trivia questions. The authors wrote in the paper: "We were surprised by this capability." It was the first time the field realized that scaling alone could produce emergent abilities.

**InstructGPT / ChatGPT (2022, 1.3B base + RLHF):** GPT-3 was powerful but uncooperative. It generated toxic text, made up facts, and ignored instructions. The fix was **Reinforcement Learning from Human Feedback (RLHF)** — a technique where humans rank model outputs, and those rankings train a reward model that fine-tunes the base model. The InstructGPT paper (Ouyang et al., 2022) showed that 1.3B parameters with RLHF could outperform 175B without. When OpenAI productized this as ChatGPT in November 2022, it reached 100 million users in two months — the fastest adoption in internet history.

**GPT-4 (March 2023):** Multimodal from the ground up. GPT-4 could accept images and text and reason across them. It scored in the 90th percentile on the bar exam, the 99th percentile on the LSAT, and 5 on 15 AP exams. OpenAI revealed almost no technical details, but leaked rumors suggested it used a mixture-of-experts architecture with ~1.8 trillion parameters and 16 experts.

## 3.2 The Great Forks: Competitors and Their Stories

The GPT lineage sparked forks in every direction. Each competitor represents a different bet on how AI should be built:

**Claude (Anthropic, 2023–):** Born from a schism. In 2021, senior OpenAI researchers — Dario and Daniela Amodei, along with seven others — left to form Anthropic, convinced that safety was being deprioritized. They developed **Constitutional AI (CAI)**, an alternative to RLHF: instead of relying on thousands of human raters, CAI uses a set of written principles to guide model behavior. Claude 3 Opus (2024) matched GPT-4 on benchmarks while using fewer parameters. Claude 3.5 Sonnet became the developer favorite for coding. By 2025, Anthropic had pushed context windows to 200K tokens — a full novel in a single prompt — and introduced "computer use" capabilities where Claude could control a desktop interface directly.

**Gemini (Google DeepMind, 2023–):** Google's counter-strike. After years of internal caution and the shocking loss of public AI leadership to OpenAI, Google merged DeepMind and Google Brain into a single unit. Gemini Ultra (December 2023) was the first model to outperform GPT-4 on MMLU (90.0% vs 86.4%). Gemini 2.5 Pro (2025) introduced "thinking mode" natively and a 1M-token context window. DeepMind's heritage — AlphaGo, AlphaFold — gave Gemini an edge in scientific reasoning.

**Llama (Meta, 2023–):** The democratization bomb. Meta released LLaMA (65B parameters) to researchers under a non-commercial license in February 2023. Within weeks, it was leaked to the public on 4chan. The floodgates opened: fine-tuned variants (Alpaca, Vicuna, WizardLM) multiplied. Meta leaned in, releasing LLaMA 2 (July 2023) with a commercial license, and LLaMA 3 (2024) at 405B parameters matching GPT-4. The open-source ecosystem — built on LLaMA's foundation — became a parallel AI universe.

**DeepSeek (China, 2024–2025):** The cost-efficiency revolution. A quiet Chinese quant-trading firm's AI lab dropped a series of models that shocked the industry. DeepSeek-V2 (2024) trained for $2.78M — roughly 1/70th of GPT-4's estimated cost. DeepSeek-V3 (2025, 671B total, 37B active per token) used an MoE architecture so efficient it trained on just over 2,000 GPUs. Then DeepSeek-R1 (January 2025) matched OpenAI's o1 at reasoning — and released the paper describing how they did it. The industry gasped. The US stock market lost $500 billion in a single day. The geopolitical narrative shifted: China was not following — it was innovating.

**The competitor landscape at a glance:**

| Lab | Origin Story | Key Innovation | Strengths | Vulnerability |
|-----|-------------|----------------|-----------|---------------|
| OpenAI | Non-profit turned capped-profit | RLHF, scaling-first, o-series reasoning | Research velocity, brand, ecosystem | Talent retention, governance instability |
| Anthropic | OpenAI safety schism (2021) | Constitutional AI, RSP framework | Safety as differentiator, coding quality | Narrow product line, slower releases |
| Google DeepMind | Merger of DeepMind + Google Brain | Native multimodality, 1M-token context | Data scale (YouTube, Images, Earth), science heritage | Bureaucracy, slow culture |
| Meta (LLaMA) | Zuckerberg's open-source bet | Open-weight licensing, ecosystem play | Community, democratization, zero licensing cost | No direct revenue model |
| DeepSeek | Chinese quant firm (High-Flyer) | MoE efficiency, cost 1/70th of GPT-4 | Cost leadership, open science, engineering culture | Geopolitical risk, hardware constraints |

Each lab placed a different bet on what would matter most: scale (OpenAI), safety (Anthropic), data (Google), openness (Meta), or efficiency (DeepSeek). The 2026 results suggest all five bets were partially correct — and the frontier belongs to those who can combine multiple advantages.

## 3.3 The Reasoning Model Breakthrough

In September 2024, OpenAI released o1 — the first model that "thinks" before answering. The rumors had called it "Strawberry" or "Q*." The reality was stranger and more important.

**How reasoning models work:**

Standard models generate the first token immediately after processing the prompt. o1 introduced **test-time compute scaling**: the model generates an internal chain-of-thought, explores multiple reasoning branches, backtracks when it hits dead ends, and verifies its own conclusions before producing a visible answer. The more compute allocated to this internal thinking, the better the results — up to a point.

This was a paradigm shift. Previously, all scaling happened at training time. Reasoning models introduced a second axis of scaling: you could dynamically trade latency and compute cost for answer quality. A hard math problem might receive 30 seconds of internal thinking; an easy question, one second.

**The reasoning model timeline:**

- **OpenAI o1-preview (September 2024):** Scored 83% on the AIME math competition (vs GPT-4's 12%). Rivaled PhD-level scientists on physics, biology, and chemistry questions.
- **OpenAI o1 full (December 2024):** Significantly better at coding and tool use.
- **DeepSeek R1 (January 2025):** Open-source. Matched o1 on math and coding. Published the full training methodology — including the "aha moment" where the model learned to re-evaluate its own approach mid-reasoning. Available for anyone to download and study.
- **o3 (February 2025):** OpenAI's next jump. Achieved 87.5% on the ARC-AGI visual reasoning benchmark — approaching human baseline. Goldman Sachs estimated its coding productivity gain at 25-30% over previous models.
- **Claude Sonnet 4 reasoning (April 2025):** Anthropic's answer. Stronger on long-context reasoning and tool orchestration.
- **Gemini 2.5 Pro "thinking" (2025):** DeepMind's natively thinking model with 1M token context.

**Why it matters:** We are no longer just scaling training compute. Reasoning models introduced **test-time compute** as a new dimension. A model can now "spend" more compute to think harder about hard problems. This changes everything — cost curves, latency trade-offs, and what we consider possible.

**The reasoning model timeline:**

| Model | Date | Test-Time Compute | AIME Score | Key Finding |
|-------|------|-------------------|-----------|-------------|
| GPT-4 | Mar 2023 | None (standard generation) | 12% | Baseline |
| o1-preview | Sep 2024 | Internal chain-of-thought | 83% | 7× improvement — reasoning is real |
| o1 full | Dec 2024 | Extended thinking | ~90% | Coding and tool use improved |
| DeepSeek R1 | Jan 2025 | Open-source reasoning | ~80% | Matched o1 at 1/20th cost; published methods |
| o3 | Feb 2025 | Multi-branch search + verification | 94% | 87.5% on ARC-AGI (approaching human ceiling) |
| Claude Sonnet 4 | Apr 2025 | Long-context reasoning | ~85% | Stronger on tool orchestration |
| Gemini 2.5 Pro | 2025 | Native thinking + 1M context | 82% | Best at long-document reasoning |

The separation between "training compute" and "inference compute" was the most important architectural shift since the transformer itself. Models could now think harder when the problem demanded it — and spend less when it didn't.

## 3.4 The Capability Trajectory

The pace of improvement between 2024 and 2025 was unlike anything in the history of technology:

| Capability | 2024 | 2025 | Change |
|------------|------|------|--------|
| SWE-bench Verified (coding) | 60% | ~100% | Saturated |
| AIME (competition math) | 12% (GPT-4) | 93% (o3) | 7.8× |
| ARC-AGI (visual reasoning) | 32% (GPT-4) | 87.5% (o3) | 2.7× |
| OSWorld (agentic tasks) | 12% | 66% | 5.5× |
| PhD-level science (GPQA) | 65% (GPT-4) | 87% (o3) | 1.3× |
| IMO (olympiad math) | Bronze | Gold | Medal upgrade |

The headline: **one year compressed a decade of expected progress.** In 2024, coding agents could solve about half of real-world GitHub issues. By 2025, they solved nearly all of them. In 2024, AI could not pass the AIME math competition. By 2025, it was scoring near the top human participants.

This trajectory shows no sign of plateauing. Each reasoning model release pushes the boundary further. The question is no longer *whether* AI will reach expert-level capability in most cognitive domains — it is *when*, and what we build with it.

### Key References

- [GPT-1 (Radford et al., 2018)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
- [GPT-2 (Radford et al., 2019)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
- [GPT-3 (Brown et al., 2020)](https://arxiv.org/abs/2005.14165)
- [InstructGPT (Ouyang et al., 2022)](https://arxiv.org/abs/2203.02155)
- [Constitutional AI (Bai et al., 2022)](https://arxiv.org/abs/2212.08073)
- [LLaMA (Touvron et al., 2023)](https://arxiv.org/abs/2302.13971)
- [GPT-4 (OpenAI, 2023)](https://arxiv.org/abs/2303.08774)
- [Gemini (Google DeepMind, 2023)](https://arxiv.org/abs/2312.11805)
- [Claude (Anthropic)](https://www.anthropic.com)
- [DeepSeek-V2 (2024)](https://arxiv.org/abs/2405.04434)
- [DeepSeek-R1 (2025)](https://arxiv.org/abs/2501.12948)
- [o1 System Card (OpenAI, 2024)](https://openai.com/index/learning-to-reason-with-llms/)
- [AIME](https://www.maa.org/math-competitions/american-invitational-mathematics-examination-aime)
- [ARC-AGI (Chollet, 2019)](https://arxiv.org/abs/1911.01547)
- [SWE-bench (Jimenez et al., 2024)](https://arxiv.org/abs/2310.06770)
