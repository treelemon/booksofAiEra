# Chapter 3: From GPT to Reasoning Models

## 3.1 The GPT Lineage

| Model | Year | Key Innovation |
|-------|------|----------------|
| GPT-1 | 2018 | Generative pre-training + fine-tuning |
| GPT-2 | 2019 | Scale reveals zero-shot transfer |
| GPT-3 | 2020 | In-context learning at 175B parameters |
| InstructGPT | 2022 | RLHF aligns model with user intent |
| GPT-4 | 2023 | Multimodal, improved reasoning |
| GPT-4o | 2024 | Native multimodality, real-time |

## 3.2 The Competitors

- **Claude (Anthropic):** Constitutional AI, safety-first design, long context
- **Gemini (Google DeepMind):** Multimodal from day one, deeply integrated
- **Llama (Meta):** Open-weight catalyst, spawned the open-source ecosystem
- **DeepSeek (China):** MoE architecture, R1 reasoning model, cost efficiency shock
- **Grok (xAI):** Real-time knowledge, less safety constraints

## 3.3 The Reasoning Model Breakthrough

2024–2025 saw a paradigm shift: models that "think" before they answer.

**How reasoning models work:**
- At inference time, the model generates an internal chain-of-thought
- It explores multiple branches, backtracks, verifies
- This "test-time compute" scales — more thinking = better answers (up to a point)

**Key models:**
- OpenAI o1 (2024) — first reasoning model
- o3 (2025) — significant improvement
- DeepSeek R1 (2025) — open-source reasoning, matched o1
- Claude Sonnet 4 reasoning (2025)
- Gemini 2.5 Pro thinking (2025)

**Implication:** We're no longer just scaling training compute. Test-time compute is a new axis of scaling. Models can now "spend" compute to think harder about hard problems.

## 3.4 The Capability Trajectory

In one year (2024→2025):
- SWE-bench Verified: 60% → ~100%
- PhD-level science questions: near-expert baselines
- Competition math: gold medal at IMO
- Tool use and agentic tasks: 12% → 66% success

The rate of improvement shows no signs of plateauing in 2026.
