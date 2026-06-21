# Chapter 4: The State of Frontier Models

## 4.1 Benchmark Snapshot (Mid-2026)

| Benchmark | Best Score | Human Baseline | Notes |
|-----------|-----------|----------------|-------|
| MMLU | 96.5% | ~90% | Multi-task language understanding |
| GSM8K | 98.2% | ~95% | Grade-school math |
| SWE-bench Verified | 97.3% | ~85% | Real-world coding tasks |
| MATH | 94.1% | ~90% | Competition mathematics |
| IMO | Gold medal | Gold medal | International Math Olympiad |
| OSWorld (agents) | 66% | ~80% | Real computer tasks |

The jagged frontier remains: PhD-level math is near-saturated, but analog clock reading is at 50.1%.

## 4.2 Frontier Model Landscape (2026)

**Closed-source leaders:**
- **Claude Opus 5** (Anthropic) — currently #1 overall
- **GPT-5** (OpenAI) — strong across all categories
- **Gemini 3 Ultra** (Google DeepMind) — multimodal leader

**Open-source / open-weight leaders:**
- **Llama 5** (Meta) — best open-weight general model
- **DeepSeek V4** (DeepSeek) — cost leader, MoE architecture
- **Olmo 3** (AI2) — fully open data + weights
- **Granite 4** (IBM) — enterprise-focused

**The gap:** Closed-source still leads by ~2.7% aggregate, but open-source is closing fast.

## 4.3 Architectural Trends

- **Mixture-of-Experts (MoE):** Most frontier models use MoE for efficiency
- **Test-time compute scaling:** Reasoning models at inference time
- **Tool use and function calling:** Native agent capabilities
- **Multimodality:** All major models are natively multimodal (text + image + audio)
- **Long context:** Standard is 128K–1M tokens

## 4.4 The Intelligence Plateau Debate

Is AI capability growth slowing? The evidence says **no**:
- Benchmarks continue to saturate (requiring new, harder ones)
- Reasoning models opened a new scaling axis
- Agentic capabilities are accelerating from a low base
- Scientific discovery applications are just beginning

The real question isn't "are we plateauing?" but "what happens when models are better than experts at everything measurable?"
