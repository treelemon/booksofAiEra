# Chapter 1: The Three Waves of AI

## 1.1 Symbolic AI (1956–2010)

The Dartmouth Conference of 1956 is conventionally cited as AI's birth. The founding belief: intelligence could be captured through explicit symbol manipulation and logical rules.

**Key milestones:**
- Perceptron (1958), ELIZA (1966), MYCIN (1976), expert systems boom (1980s)
- AI winters (1974–1980, 1987–1993)
- Deep Blue defeats Kasparov (1997)

**What went right:** Rule-based systems excelled in narrow, well-defined domains (chess, medical diagnosis).
**What went wrong:** Symbolic AI couldn't handle ambiguity, uncertainty, or the messiness of real-world perception and language. Hand-crafted rules don't scale.

## 1.2 Statistical ML (2010–2020)

The shift from hand-coded rules to learned patterns from data. Three ingredients converged: the internet (data), GPUs (compute), and backpropagation (algorithm).

**Key milestones:**
- ImageNet breakthrough (AlexNet, 2012)
- Word2vec (2013), seq2seq + attention (2014)
- GANs (2014), AlphaGo (2016), BERT (2018)

**What went right:** Statistical methods crushed symbolic approaches on perception tasks (vision, speech, translation).
**What went wrong:** Each model was narrow — you trained a separate model for each task. No common sense, no transfer, no reasoning.

## 1.3 Foundation Models (2020–Present)

The unification: one model trained on internet-scale data, adaptable to hundreds of tasks without retraining.

**Key milestones:**
- GPT-3 (2020), DALL-E (2021), ChatGPT (2022)
- GPT-4, Claude, Gemini, Llama (2023–2024)
- Reasoning models: o1, o3, DeepSeek R1 (2024–2025)
- Agentic AI (2025–2026)

**What's different:**
1. **Scale** — parameters, data, compute all grew 1000x+
2. **Emergence** — capabilities appear at scale that weren't explicitly trained for
3. **Generality** — one model does text, code, images, audio, reasoning
4. **Continuity** — no more AI winters; this wave is self-reinforcing

## Key Takeaways

Each wave built on the last. The pendulum swung from rules to statistics to scale. Understanding this history inoculates you against two mistakes: thinking AI is "just pattern matching" (it's more than that now) and thinking it's "basically human" (it's not that either).
