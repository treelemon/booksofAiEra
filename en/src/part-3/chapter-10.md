# Chapter 10: Open-Source vs. Closed-Source

## 10.1 The Leak That Started a Revolution

In February 2023, Meta released **LLaMA** — a family of language models from 7B to 65B parameters — to approved academic researchers under a non-commercial license. The intention was responsible research. The outcome was the opposite.

Within weeks, the model was leaked to 4chan. Anyone with internet access could download LLaMA and run it on their own hardware. The cat was out of the bag — and would never go back in.

**Mark Zuckerberg**, Meta's CEO, faced a decision: sue the leakers, tighten security, and kill the project — or lean in. He leaned in. "Open-source AI is the best path forward," Zuckerberg wrote in July 2023, announcing LLaMA 2 with a commercial license. "Everyone should have access to the benefits of AI."

The decision was a masterstroke. Within a year, the LLaMA ecosystem — fine-tuned variants like Alpaca, Vicuna, and WizardLM — had spawned a parallel AI universe. By 2025, there were over 50,000 LLaMA-based models on Hugging Face. Meta had not built an AI product. It had built an AI *operating system*.

**Yann LeCun**, Meta's chief AI scientist, became the most vocal champion of open-source AI. He debated anyone who would listen — arguing that open-source would win because "innovation accelerates when everyone can participate." His favorite foil was **Eliezer Yudkowsky**, who argued that open-source models were an existential risk because "there will be no 'off switch' for a misaligned AI if the weights are public."

The schism ran through every lab, every company, and every government.

## 10.2 The DeepSeek Watershed

January 2025 was the moment the debate crystalized.

DeepSeek-R1 matched OpenAI's o1 on reasoning benchmarks — and published the full training methodology. The weights were downloadable. The paper was readable. The cost was $6 million, not $200 million.

**Liang Wenfeng**, DeepSeek's founder, had not set out to make a political point. He had simply built the most efficient model architecture in the world. But the political implications were unavoidable: DeepSeek proved that frontier AI could be built by anyone with engineering talent and $6 million — not just the trillion-dollar tech companies.

The effects rippled across the industry:
- **China's AI ecosystem exploded.** GLM-5 (Zhipu AI), Kimi K2 (Moonshot AI), and ByteDance's Doubao all released open-weight models within months.
- **OpenAI released its first open model** in August 2025 — a small but capable reasoning model. The company that had started as a non-profit "for the benefit of humanity" had been forced back toward its founding mission by competitive pressure.
- **The US government struggled to respond.** Export controls on chips could slow China's frontier development. But what could you control when all the software was free?

## 10.3 The Two Camps in 2026

The open-source ecosystem had matured into distinct tiers by 2026:

**The General-Purpose Leaders:**
- **Llama 5 (Meta):** The crown jewel of open-weight. 600B parameters with dual-pass inference architecture. Matched GPT-5 on most benchmarks. The license was permissive enough for most commercial use. Meta's strategy: give away the model, own the ecosystem.
- **DeepSeek V4 (DeepSeek):** 1.2T total, 37B active per token. The efficiency leader. Continued the tradition of detailed technical reports that advanced the entire field.

**The Fully Open Movement:**
- **Olmo 3 (AI2, led by Ali Farhadi):** The gold standard for openness — not just weights, but full training data, code, logs, and recipes. If you wanted to know *exactly* how a frontier model was built, Olmo was your only choice.
- **Granite 4 (IBM):** Enterprise-focused with a permissive license designed for regulated industries. Auditable training data, contractual guarantees against IP infringement.

**The European Contingent:**
- **Mistral Large 3 (Mistral):** Founded by **Arthur Mensch**, **Guillaume Lample**, and **Timothée Lacroix** — all former DeepMind and Meta researchers. Mistral had become Europe's AI champion by combining open-source ethos with a sustainable business model. Le Chat, their consumer product, was Europe's only native frontier AI assistant.

**The Small but Mighty:**
- **Phi-4 (Microsoft):** 14B parameters that punched far above its weight. Designed for edge deployment — running on laptops and phones.

## 10.4 The Licenses War

Behind the model performance was a subtler war: **what does "open-source" mean for AI?**

The Open Source Initiative (OSI) had spent 2024 defining "Open Source AI" — and the process was contentious. The traditional definition (OSD) required that anyone could use the software for any purpose. But AI models had a complication: they were not just code. They were *weights*, *data*, *training code*, and *hardware requirements*.

Three licensing camps emerged:

1. **Open weights + restrictive use (Apache 2.0 with use-case restrictions):** Llama's license banned "high-risk" uses — weapons, surveillance, bioweapons. Critics said this was not true open source.
2. **Fully open (Apache 2.0, no restrictions):** Olmo and Granite used traditional permissive licenses. Maximum openness, maximum potential for misuse.
3. **Open weights, closed data (custom licenses):** DeepSeek published weights and architecture but kept training data proprietary. Trade secrets and competitive advantage.

The OSI eventually approved a definition that required *data transparency* for a model to be called "Open Source AI" — but the debate continued. **Ali Farhadi** (AI2) argued: "If you can't inspect the training data, you can't audit the model. It's not open source — it's open weights." **Mark Zuckerberg** countered: "Perfect openness is the enemy of good openness. Open weights with reasonable restrictions is the pragmatic path."

## 10.5 The Safety Schism

The deepest divide was not technical — it was philosophical.

**The open-source safety case (Yann LeCun, Mark Zuckerberg, Liang Wenfeng):**
- Transparency allows security researchers to find and fix vulnerabilities
- Distributed capability prevents single-point-of-failure concentration
- Public scrutiny is the best mechanism for alignment research
- Closed models create a dangerous asymmetry: the rich control AI, the rest consume it

**The closed-source safety case (Dario Amodei, Sam Altman, Eliezer Yudkowsky):**
- Powerful AI in the wrong hands is an existential risk
- Open weights cannot be recalled if they enable bioweapons or autonomous warfare
- Centralized control enables safety interventions (monitoring, fine-tuning, shutdown)
- Democracy requires that powerful technology be governed, not distributed

**The middle ground (Demis Hassabis):**
- Safety requirements should scale with capability
- Current open models are safe enough; future ones may need regulation
- The right approach is tiered: open for research, regulated for deployment

The debate had real consequences. In 2025, Meta commissioned a third-party safety audit of Llama 5 before release — a first for open-weight models. The audit revealed several attack vectors that Meta fixed before launch. Open-source advocates pointed to this as proof that transparency works. Closed-source advocates pointed out that Llama 5 still had vulnerabilities that a motivated adversary could exploit.

## 10.6 The Coexistence Thesis

By 2026, it was clear that neither side would win. The two models were not competing — they were complementing.

Open-source dominated:
- **Research and science:** Academic labs could not afford API access at scale. Open models were the only practical option.
- **Education and learning:** Students and self-learners downloaded, studied, and modified open models.
- **Global South:** Countries without the infrastructure for API-based AI relied on locally-hosted open models.
- **Specialized domains:** Healthcare, legal, and financial applications fine-tuned open models on private data.

Closed-source dominated:
- **Enterprise production:** Companies paid for reliability, support, SLAs, and indemnification.
- **Safety-critical applications:** Regulated industries preferred models with known provenance and audit trails.
- **Consumer products:** Seamless API access, no infrastructure management.

The 2.7% gap in aggregate benchmarks was still real. But in practice, for most applications — coding, writing, analysis, customer service — open-source models were already good enough.

**Yann LeCun** was right about one thing: open-source won. Not in the sense of defeating closed-source, but in the sense that AI had become like the internet — a technology that no single company could control, even the companies that made it.
