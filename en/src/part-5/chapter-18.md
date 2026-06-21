# Chapter 18: The Path to AGI

## 18.1 The AGI Definition Matrix

In December 2024, François Chollet posted a screenshot of a benchmark score. His ARC-AGI benchmark — designed to measure general intelligence in AI systems — had been sitting at a human baseline of 85% for years. The best AI scored 30%. Then o3 scored 87.5%. The tweet went viral. "AGI has been achieved," some declared. "No it hasn't," others responded. "The benchmark is saturated."

Both sides were right — according to their own definitions.

Before the debate about *when* AGI arrives comes a more fundamental question: *what* counts as AGI? The field has no consensus definition — and the definition you choose determines your timeline, your risk assessment, and your deployment strategy.

**A professional AGI definition taxonomy:**

| Definition Type | Definition | Implied Timeline | Risk Profile | Proponents |
|-----------------|------------|------------------|--------------|------------|
| **Economic** | Any economically valuable work at or above human level | Already partially realized | Deployment risk (rushing without safety) | Sam Altman, tech executives |
| **Cognitive** | Matches or exceeds human performance on all cognitive tasks | 5-15 years | Alignment risk (capabilities outpace safety) | AI researchers, safety researchers |
| **Generality** | Learn any novel task from scratch with no pre-training | 15-30+ years | Robustness risk (brittle in unfamiliar contexts) | François Chollet, cognitive scientists |
| **Recursive self-improvement** | AI improves its own architecture and training | 3-8 years after any definition is met | Existential risk (unauditable acceleration) | Eliezer Yudkowsky, safety community |
| **Operational** | "The last tool you ever need to build" (Sriram Krishnan) | Depends on other definitions | Loss of control risk | Silicon Valley investors |

No single definition is correct. The professional approach is to track all five definitions separately. When someone says "AGI is N years away," the first question should always be: which definition are you using? A model that passes the economic definition may still be decades from the generality definition. Chollet's benchmark was not the end of the debate — it was proof that the debate needed better definitions.

## 18.2 The Capability Assessment Framework

In 2023, GPT-4 passed the bar exam in the 90th percentile. In 2024, o3 passed GPQA Diamond — a PhD-level science test — at 87.4%, exceeding human experts. In 2025, reasoning models matched top competitors on the AIME math competition.

Each of these milestones triggered a wave of "AGI is here" announcements. Each was followed by a demonstration of failure: a simple reasoning problem the model could not solve, a basic fact it got wrong, a logical contradiction it did not notice.

The pattern reveals a truth about capability assessment: benchmarks show what AI *can* do, not what it *understands*.

**The AGI capability scorecard (2026):**

| Capability | Current State | AGI Threshold | Gap |
|------------|---------------|---------------|-----|
| **Mathematical reasoning** | o3: 83% AIME | 90%+ (human expert) | 7 points |
| **Scientific reasoning** | o3: 87.4% GPQA Diamond | 80%+ (PhD-level) | PASSED |
| **General intelligence** | o3: 87.5% ARC-AGI | 85%+ (human ceiling) | PASSED (new harder benchmark needed) |
| **Code generation** | 25-50% SWE-bench | 80%+ (senior engineer) | 30-55 point gap |
| **Visual understanding** | GPT-4o: 87% MMMU | 90%+ (expert level) | 3-10 points |
| **Long-context reasoning** | 95%+ at 100K tokens | 99.9% at 1M+ | Significant |
| **Planning & execution** | 12-40% OSWorld | 80%+ | 40-68 point gap |
| **Continuous learning** | Fine-tuning required | Learn from 0 examples | Fundamental gap |
| **Meta-cognition** | Partial self-evaluation | Accurate self-assessment | Improving with o-series |
| **Theory of mind** | Basic tests passed | Human-level social reasoning | Significant gap |

**The aggregate AGI readiness score across all dimensions: approximately 45-55 out of 100.** The ceiling effect means benchmark scores plateau even as genuine capability gaps remain. The professional evaluator tracks not just whether benchmarks are passed, but whether new benchmarks reveal structural weaknesses — which they always do.

## 18.3 The Scaling Assessment

The scaling hypothesis — that increasing compute, data, and parameters produces AGI — has been the field's dominant framework. In December 2024, it faced its most rigorous test. DeepSeek released V3: a model trained for $5.6 million that matched GPT-4's performance. GPT-4 cost an estimated $200 million to train. DeepSeek achieved parity at 1/35th the cost.

"I don't know if scaling leads to AGI," one researcher said. "But I know that the cost of finding out is dropping rapidly — and that means more people will try."

**The scaling evaluation framework:**

| Variable | GPT Series (2018-2023) | DeepSeek (Dec 2024) |
|----------|----------------------|-------------------|
| Parameters | 117M → 1.8T (15,000×) | 2.3T (expert ensemble) |
| Training cost | ~$4.6M (GPT-3) → ~$200M (GPT-4) | $5.6M |
| Performance | Benchmark leader each generation | Match at 97% less cost |

**The three observations:**

1. **The scaling curve is not smooth.** The jump from GPT-3 to GPT-4 was dramatic (~20× compute). The jump from GPT-4 to GPT-4o was modest (<2×). The jump in reasoning (GPT-4o → o1) came from algorithmic innovation, not scale.

2. **Efficiency gains are real and consequential.** DeepSeek's achievement means the compute threshold for AGI-relevant capabilities is dropping, not rising. This increases deployment risk even as it democratizes access.

3. **The marginal returns are debated.** A 25,000× increase from GPT-1 to GPT-4 produced dramatic gains. Another 100× would cost $20+ billion. The critical unknown is whether the next leap is another transformation or diminishing returns.

## 18.4 The Reasoning Breakthrough

September 2024. OpenAI released o1 — not just a new model, but a new paradigm. Instead of predicting the next token, the model "thought" before answering. It generated chains of reasoning, explored alternatives, and checked its own work. The results were startling: AIME math scores jumped from 12% to 83% — a 7× improvement in one release.

"This is not an incremental improvement," Ilya Sutskever had said earlier. "This is a new capability."

**Reasoning model performance matrix (2025-2026):**

| Benchmark | GPT-4o | o1 | o3 | DeepSeek R1 | Gemini Thinking |
|-----------|--------|----|----|-------------|-----------------|
| AIME (math) | 12% | 83% | 94% | 80% | 82% |
| GPQA Diamond (PhD science) | 56% | 78% | 87% | 71% | 75% |
| ARC-AGI (general) | 30% | ~50% | 87.5% | ~45% | ~48% |
| Codeforces (competitive) | ~10th pct | top 500 | top 200 | top 400 | top 300 |
| SWE-bench (code tasks) | ~15% | ~25% | ~40% | ~30% | ~35% |

**The four key findings:**

1. **Reasoning is quantifiable.** The AIME jump from 12% to 83% was not hype. These are real, measurable gains.

2. **The test-time compute trade-off exists.** o3 at its highest reasoning setting can cost $10+ per query. The model does not "think better" for free; it thinks more expensively.

3. **Open-source parity arrived within 4 months.** DeepSeek R1 matched o1's reasoning in January 2025. Reasoning techniques are not proprietary moats — they spread rapidly.

4. **The "reasoning = understanding" fallacy.** A model scoring 87% on GPQA can generate correct answers to PhD-level questions without understanding physics. It has learned to generate sequences of tokens that appear in training data for correct answers. The professional verification methodology applies to every reasoning model output, regardless of benchmark scores.

## 18.5 The Six Paths Decision Matrix

| Criterion | Scale | Reasoning | Agents | New Architecture | Embodied | Neuro-Symbolic |
|-----------|-------|-----------|--------|-----------------|----------|----------------|
| **Evidence strength** | Strong | Strong | Moderate | Weak | Moderate | Weak |
| **Compute required** | Very high | High | Moderate | Low | High | Moderate |
| **Path clarity** | Clear trajectory | Clear metrics | Practical | Theoretical | Intuitive | Conceptual |
| **Safety** | Centralized | Centralized→Distributed | Distributed | Unknown | Moderate | Favorable |
| **Leading proponents** | Altman, Amodei | Sutskever, DeepSeek | Adept, Cognition | MIT, Stanford | LeCun, Malik | Tenenbaum, Marcus |
| **Year estimate** | 2028-2032 | 2027-2030 | 2028-2035 | 2030-2040 | 2035-2050 | 2030-2045 |

The six paths are not mutually exclusive. The most likely outcome is a hybrid: scale provides base capability, reasoning provides accuracy, agents provide utility, and some combination provides robustness. The professional strategist should not bet on a single path but build capability across multiple.

## 18.6 The Timeline Aggregation

Geoffrey Hinton's observation captures the uncertainty: "The timeline question is not answerable — and the fact that we cannot answer it is itself the answer."

Uncertainty about AGI is structural, not epistemic. We cannot resolve it by gathering more data. The proper response is not a single prediction but a strategy robust to a wide range of arrival dates.

**Methodology for aggregating expert forecasts:**

1. Collect multiple survey sources (AI Impacts 2023: median 2059; Dynabench 2024: median 2047; Expert surveys 2025: median 2039; Superforecasters 2025: median 2042)
2. Adjust for known biases: professional bias (weight academic 2×), incentive bias (CEOs claim near-term), availability bias (recent breakthroughs distort perception)
3. Compute the implied distribution: 10th percentile 2028-2030, 25th 2032-2035, 50th 2039-2042, 75th 2047-2055, 90th 2065+
4. Apply the asymmetry principle: the cost of underestimating (AGI arrives sooner, unprepared) is far higher than overestimating. Prudent planning uses the 25th percentile timeline — not the median.

## 18.7 The AGI Readiness Framework

| Dimension | Current State (2026) | Target | Gap |
|-----------|---------------------|--------|-----|
| Safety research investment | ~$500M/year | $5-10B/year | 10-20× |
| Alignment techniques | RLHF, Constitutional AI | Robust, scalable alignment | Unsolved at superhuman levels |
| Governance infrastructure | EU AI Act, voluntary declarations | Binding international treaty | Early stage |
| Regulatory capacity | ~200 regulators | 5,000+ with technical expertise | 25× |
| Interpretability research | Neuron-level mapping | Circuit-level understanding | Decades behind |
| Red-teaming capacity | Thousands of humans | Millions+ | Supply constrained |
| Public AI literacy | 38% detect deepfakes | 90%+ | Massive gap |

**The professional action framework:** Short-term (1-2 years): support alignment research; adopt AI risk evaluation standards; build AI literacy. Medium-term (3-5 years): develop interpretability or alignment evaluation expertise; participate in governance standard-setting. Long-term (5-10 years): contribute to institutional infrastructure for managing transformative AI.

## 18.8 The AGI That Already Exists

In 1976, Joseph Weizenbaum — creator of the ELIZA chatbot — wrote: "The question is not whether machines can think. The question is whether humans can think clearly about machines."

Fifty years later, the question has not changed. If AGI is an economic threshold — performing any economically valuable work at human level — then it has arguably arrived for thousands of tasks. If AGI is a cognitive threshold — thinking, feeling, understanding like a human — then it remains distant.

The professional perspective holds both truths simultaneously:

- **De facto AGI:** AI systems now exceed human capability in specific domains (medical image diagnosis, legal document analysis, code generation, mathematical reasoning). The decision to call this "AGI" is semantic. The operational reality is that these systems replace human judgment in their domains.

- **De jure AGI:** No system exhibits the generality, flexibility, robustness, or understanding of a human being. Every current AI is narrow in practice — excelling in its training distribution, failing outside it.

The most dangerous mistake is conflating these two senses. If we believe AGI has arrived (economic sense), we may deploy recklessly in domains where the system lacks true understanding. If we believe AGI has not arrived (cognitive sense), we may fail to prepare for systems that already make high-stakes decisions.

The path of **Human Wisdom** is to acknowledge both truths: to use AI's current capabilities with full awareness of their limits, while preparing for a future where those limits expand — potentially suddenly. The path to AGI is not a technological inevitability. It is a human choice — made through every deployment decision, every safety investment, every governance framework. That choice, not the algorithm, will determine what AGI becomes.
