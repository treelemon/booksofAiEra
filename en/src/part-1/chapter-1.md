# Chapter 1: The Three Waves of AI

*Every technology has its creation myth. AI's begins in the summer of 1956, on the campus of Dartmouth College, where a small group of men gathered to build a god.*

---

## 1.1 The First Wave: Symbolic AI (1956–2010)

### The Summer of Big Dreams

In August 1956, John McCarthy, Marvin Minsky, Claude Shannon, and four others convened for a six-week workshop at Dartmouth. Their proposal was audacious:

> *"Every aspect of learning or any other feature of intelligence can in principle be so precisely described that a machine can be made to simulate it."*

They called it "artificial intelligence." The term itself was a strategic choice — neutral enough to avoid the stigma of cybernetics, ambitious enough to attract funding. It worked.

The early results were electric. In 1958, Frank Rosenblatt built the **Perceptron** at Cornell, a neural network that could learn to recognize visual patterns. The New York Times called it "the first serious rival to the human brain." The US military poured millions into "thinking machine" research.

In 1966, MIT's Joseph Weizenbaum created **ELIZA**, a chatbot that simulated a Rogerian psychotherapist. To his horror, people treated it as human. His secretary asked him to leave the room so she could speak to ELIZA in private. Weizenbaum became one of AI's earliest critics, warning that people would mistake simulation for understanding.

### The First Winter

By the early 1970s, the promises had overshot reality. Machine translation was a disaster — a famous example translated "the spirit is willing but the flesh is weak" into Russian and back as "the vodka is good but the meat is rotten." The US government's Lighthill Report (1973) was devastating: AI had failed to deliver on its grand promises.

Funding evaporated. The first AI winter had begun.

### The Expert System Boom

The field found its second wind in the 1980s with **expert systems** — programs that encoded human expertise into thousands of hand-crafted rules. **MYCIN** (1976) diagnosed blood infections as well as Stanford doctors. **XCON** (1980) saved DEC $40M annually configuring computer systems.

The Japanese government launched the Fifth Generation Computer project (1982), pledging billions to build a revolutionary AI. The US responded with its own strategic computing initiative.

### The Second, Deeper Winter

The Fifth Generation project failed. Expert systems turned out to be brittle — they worked in laboratories but collapsed under the complexity of the real world. Each rule had to be handwritten. There was no learning, no adaptation, no common sense.

By 1987, the market for AI hardware collapsed. Japan's Fifth Generation was quietly abandoned. Another AI winter set in — this one so cold that researchers began renaming their work to avoid the taint of "AI." It became "machine learning." It became "data science." It became "statistics."

Some of the best minds in AI spent the 1990s in the wilderness.

### The Chess Victory — and a Lesson

In 1997, IBM's **Deep Blue** defeated world champion Garry Kasparov. It was front-page news: "The brain's last stand." But Deep Blue was not intelligent in any meaningful sense. It evaluated 200 million positions per second using brute-force search and custom hardware. It was a savant — breathtakingly narrow, incapable of learning, useless at anything except chess.

The public was awed. AI researchers were worried. If brute-force search was the path, we were on the wrong road entirely.

The second wave was already brewing, unnoticed by most.

---

## 1.2 The Second Wave: Statistical ML (2010–2020)

### The Bet That Changed Everything

In 2009, a Stanford professor named **Fei-Fei Li** decided that AI needed to see the world. She built **ImageNet** — 14 million labeled images spanning 20,000 categories, assembled through Amazon Mechanical Turk at enormous effort. Most researchers thought she was wasting her time. "We already have enough data," they told her.

In 2012, a team led by **Alex Krizhevsky, Ilya Sutskever, and Geoffrey Hinton** entered the ImageNet competition with a deep neural network called **AlexNet**. They crushed the competition — their error rate was 15.3%, the next best was 26.2%. It was not an improvement. It was a revolution.

The key insight: three ingredients had finally converged. The **internet** provided data. **NVIDIA GPUs** provided compute — Hinton had bought two from a computer store in Toronto. And **backpropagation**, the algorithm invented decades earlier, finally had enough scale to work.

### The Cambrian Explosion

The dam broke. In rapid succession:

- **2013:** Tomas Mikolov at Google released **Word2vec**, showing that words could be represented as vectors with astonishing semantic properties. "King - man + woman = queen." The machine had learned meaning from statistics.

- **2014:** **Generative Adversarial Networks (GANs)** were born from a bar bet. Ian Goodfellow, then a PhD student, argued with friends that a network could generate realistic images. He went home, coded it that night, and it worked. "The most important idea in the last 20 years of AI," Yann LeCun would call it.

- **2016:** **AlphaGo** defeated Lee Sedol, the world's greatest Go player. The match's second game produced **Move 37** — a play so unexpected that it was initially assumed to be a mistake. It wasn't. For the first time, AI had done something *creative*, something no human would have done. Lee Sedol called it "beautiful."

- **2018:** **BERT** (Google) transformed natural language understanding. It could answer questions, analyze sentiment, and understand context — not perfectly, but at a level no one had achieved before.

### What the Second Wave Could Not Do

For all its triumphs, this wave had a fundamental flaw: **narrowness**. You trained a separate model for translation, a separate model for image recognition, a separate model for question answering. There was no transfer. No common sense. No reasoning.

Each model was a brilliant idiot savant.

The phrase "AI" was still largely misleading. What people called AI was really a collection of specialized pattern-matchers, each one useless outside its training domain.

But the third wave was already visible on the horizon.

---

## 1.3 The Third Wave: Foundation Models (2020–Present)

### The Scaling Revelation

In 2020, OpenAI released **GPT-3** — 175 billion parameters trained on most of the public internet. It could write poetry, answer questions, generate code, translate languages, and do things its creators had never anticipated.

The key discovery was **in-context learning**: GPT-3 could learn to perform a new task from just a few examples in the prompt, without any weight updates. No one had designed this capability. It had *emerged* from scale.

Kaplan et al. (2020) published the scaling laws: model performance follows a predictable power law as you increase parameters, data, and compute. The implication was breathtaking: **there was no ceiling in sight.**

### The Generative Explosion

- **2021:** OpenAI's **DALL-E** generated images from text descriptions. For the first time, AI could create visual art from imagination.
- **2022:** **ChatGPT** reached 100 million users in two months — the fastest adoption in history. AI went from research curiosity to mainstream utility overnight.
- **2023:** **GPT-4** passed the bar exam (scoring in the 90th percentile), the SAT, and multiple AP exams. Microsoft's Satya Nadella called it a "platform shift as significant as the PC, the web, and the smartphone."

### The Great Open-Source Revolt

In February 2023, Meta released **Llama** to researchers under a non-commercial license. Within weeks, the model was leaked to the public. A global ecosystem exploded: fine-tuned variants, quantized versions running on laptops, specialized models for medicine, law, coding.

DeepSeek's **R1** (January 2025) proved that frontier-level reasoning could be achieved at 10–20% of the cost of closed models. The gap between open and closed collapsed.

### The Reasoning Breakthrough

In 2024, OpenAI released **o1** — the first reasoning model. Instead of immediately answering, it generates an internal chain of thought, explores multiple branches, backtracks, and verifies its conclusions. This "test-time compute" scaling opened a new axis of improvement.

By 2025, **o3**, **DeepSeek R1**, and **Claude reasoning** had made test-time thinking standard. On SWE-bench, a coding benchmark that measures real-world software engineering, AI went from 33% to 97% in two years.

### The Agentic Turn

2025–2026 marked a new phase: AI that doesn't just respond, but **acts**. Autonomous agents that plan, use tools, execute code, and persist across long tasks. OSWorld task success jumped from 12% to 66% in a single year.

We are still in the early days of this wave.

---

## Key Takeaways — The Story So Far

Three waves, each built on the last:

| Wave | Core Idea | Time Span | Key Enabler | Peak | Limitation | Legacy |
|------|-----------|-----------|-------------|------|------------|--------|
| Symbolic AI | Hand-coded rules | 1956–2010 | Logic, expert knowledge | Expert systems (1980s) | Brittleness — rules don't scale | Proved AI was possible; established reasoning as a goal |
| Statistical ML | Learned patterns from data | 2010–2020 | Internet data, GPUs, backprop | Deep learning (2010s) | Narrowness — each model solves one task | Proved learning worked better than programming |
| Foundation Models | Large-scale pre-training | 2020–Present | Transformer, scaling laws | GPT-4 + reasoning (2024–2025) | Truthfulness, alignment, control | Proved that scale + data + compute produces emergence |

The pendulum swung from **rules** to **statistics** to **scale**. Each wave seemed insurmountable in its moment, then collapsed into the seed of the next.

**The wave framework for professional analysis:**

```
For any AI technology, ask:
  1. Which wave does it belong to? (symbolic, statistical, or foundation?)
  2. What is its core mechanism? (rules, patterns, or scale?)
  3. What is its current limitation? (brittleness, narrowness, or alignment?)
  4. What would the next wave need to overcome this limitation?
```

This framework is not historical trivia. It is a practical tool for evaluating any new AI claim: identify which wave it belongs to, check whether the limitation of that wave has been solved, and assess whether the claim is real progress or a re-labeling of old ideas.

**What this history teaches us:**
- Every apparent limitation of today's AI is a future breakthrough waiting to happen
- The human tendency is to overestimate what AI can do in the short term and underestimate it in the long term — we've done this three times
- The most important capabilities of the next wave will be ones we didn't explicitly design

The most dangerous mistake is not thinking AI is too powerful. It's thinking AI is "just a pattern matcher" — and missing that pattern matching, at sufficient scale, begins to look a lot like understanding.

### Key References

- Dartmouth workshop: https://en.wikipedia.org/wiki/Dartmouth_workshop
- Perceptron (Rosenblatt, 1958): https://en.wikipedia.org/wiki/Perceptron
- ELIZA (Weizenbaum, 1966): https://en.wikipedia.org/wiki/ELIZA
- Lighthill Report (1973): https://en.wikipedia.org/wiki/Lighthill_report
- Deep Blue (IBM, 1997): https://en.wikipedia.org/wiki/Deep_Blue_(chess_computer)
- ImageNet (Fei-Fei Li, 2009): https://en.wikipedia.org/wiki/ImageNet
- AlexNet (Krizhevsky et al., 2012): https://dl.acm.org/doi/10.1145/3065386
- Word2vec (Mikolov et al., 2013): https://arxiv.org/abs/1301.3781
- GANs (Goodfellow, 2014): https://arxiv.org/abs/1406.2661
- AlphaGo (DeepMind, 2016): https://en.wikipedia.org/wiki/AlphaGo
- BERT (Devlin et al., 2018): https://arxiv.org/abs/1810.04805
- GPT-3 (Brown et al., 2020): https://arxiv.org/abs/2005.14165
- Scaling Laws (Kaplan et al., 2020): https://arxiv.org/abs/2001.08361
- DALL-E (Ramesh et al., 2021): https://arxiv.org/abs/2102.12092
- ChatGPT (OpenAI, 2022): https://openai.com/blog/chatgpt/
- LLaMA (Touvron et al., 2023): https://arxiv.org/abs/2302.13971
- GPT-4 (OpenAI, 2023): https://arxiv.org/abs/2303.08774
- DeepSeek-R1 (2025): https://arxiv.org/abs/2501.12948
