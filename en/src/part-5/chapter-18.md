# Chapter 18: The Path to AGI

## 18.1 The Word That Split the World

In November 2023, a mysterious message circulated among OpenAI's board of directors. The company had achieved a breakthrough — a model internally codenamed **Q\* (Q-Star)** that could solve mathematical problems it had never seen before. To some board members, this was not a cause for celebration. It was a reason to fire the CEO.

When Sam Altman was abruptly ousted on November 17, 2023, the stated reason was "not consistently candid in his communications." But the rumor that spread through Silicon Valley was different: the board believed Q* was a step toward AGI, and Altman was moving too fast. **Ilya Sutskever**, OpenAI's chief scientist and a board member, had become convinced that the company's approach was reckless.

Sutskever had co-founded OpenAI in 2015 with a single mission: build AGI safely. By late 2023, he believed the AGI part was succeeding faster than expected — and the safety part was failing.

"Ilya has spent his entire career thinking about what happens when AI becomes smarter than humans," a former OpenAI researcher told the press. "When he saw Q*, he didn't see a product. He saw a warning."

Altman was reinstated five days later. Sutskever was marginalized. In May 2024, he left OpenAI to found **Safe Superintelligence Inc. (SSI)** — a company with a single goal: build safe superintelligence, with no product distractions.

The question that split the most important AI company in the world is the same question this chapter must confront: **What is AGI, how close are we, and what happens when it arrives?**

## 18.2 The Definitions That Divided a Field

There was no consensus on what AGI meant. Every expert had a different definition — and each definition implied a different timeline.

**The economic definition:** An AI that can perform any economically valuable work at human level. This was Sam Altman's operating definition — AGI was whatever created enough economic value to make everything else obsolete. By this measure, some already considered GPT-4 and its successors "narrow AGI" in specific domains.

**The cognitive definition:** An AI that matches or exceeds human performance on all cognitive tasks. This was the traditional AI research definition — a system that could reason, plan, learn, and adapt like a human. By this measure, no existing system came close.

**The generality definition:** An AI that can learn any task from scratch, with no pre-training, no fine-tuning, and no special architecture. This was the hardest test — the one that measured not just performance but flexibility.

**Srinivas's pragmatic definition:** The venture capitalist **Sriram Krishnan** captured the Silicon Valley mood: "AGI is just the last tool you ever need to build." Once AI could design and build better AI, the human role shifted from creator to curator.

**The "Human Wisdom" framing:** Definitions were not neutral. They encoded values. If you defined AGI as economic productivity, you prioritized speed. If you defined it as human-like cognition, you prioritized alignment. If you defined it as general learning, you prioritized robustness. The definition you chose determined the risks you accepted. The question was not just "can we build AGI?" — it was "what kind of AGI do we want to build?"

## 18.3 The "Sparks" Paper That Changed the Conversation

In March 2023, a team of Microsoft researchers led by **Sébastien Bubeck** published a paper titled *"Sparks of Artificial General Intelligence: Early experiments with GPT-4."* The paper was unprecedented: Microsoft's research division, which had invested billions in OpenAI, was claiming that GPT-4 showed "sparks of AGI."

The evidence was striking. GPT-4 could:
- Write code, explain it, debug it, and optimize it
- Generate creative stories with consistent characters and plots
- Solve novel math problems it had never encountered
- Understand humor, sarcasm, and social context
- Reason about its own reasoning (meta-cognition)

Bubeck's paper went viral — and sparked intense backlash. Critics pointed out that GPT-4 still made basic errors, hallucinated facts, and lacked genuine understanding. "A parrot with better pattern matching is not AGI," **Gary Marcus** wrote. But the paper had shifted the Overton window. Before March 2023, saying "GPT shows sparks of AGI" was fringe. After, it was a legitimate debate.

**The "Human Wisdom" insight:** The sparks paper revealed something important about human psychology — our tendency to anthropomorphize. When a model seemed to think, we assumed it was thinking. But GPT-4 had no internal experience, no consciousness, no understanding. It was an astonishingly sophisticated pattern recognizer. The "sparks" were in the eye of the beholder. And that was the danger: if we mistook simulation for sentience, we would make catastrophic errors in judgment.

## 18.4 The Scaling Story

The dominant narrative of AI progress from 2017 to 2024 was simple: **scale was all you needed.**

**The bitter lesson:** In 2019, **Rich Sutton**, one of AI's founding figures, published an essay that became the field's unofficial manifesto. "The bitter lesson," he wrote, "is that general methods that leverage computation are the most effective, and by a large margin." Human-engineered knowledge and domain-specific tricks were temporary shortcuts. The real path to intelligence was bigger models, more data, and more compute.

For seven years, the bitter lesson held. GPT-1 (117M parameters, 2018) → GPT-2 (1.5B, 2019) → GPT-3 (175B, 2020) → GPT-4 (estimated 1.8T, 2023). Each leap in size produced a leap in capability.

**The chinchilla reversal (2022):** DeepMind's **Hoffmann et al.** paper showed that most models were undertrained — they had too many parameters and not enough data. The optimal approach was smaller models trained on more data. This "Chinchilla scaling law" reshaped the industry. Every lab changed its training strategy.

**The scaling debate:** By 2025, the consensus had fractured. Some — like **Dario Amodei** (Anthropic) and **Sam Altman** (OpenAI) — believed that scaling would continue to yield returns, with AGI arriving within 3-5 years. Others — like **Yann LeCun** (Meta) and **François Chollet** (Google) — argued that scaling alone would hit a wall. "Scaling gives you better parrots, not AGI," Chollet said. LeCun predicted AGI was "decades away."

**The DeepSeek disruption (December 2024):** DeepSeek released a model that matched GPT-4 at 1/20th the training cost — $5.6 million vs. an estimated $100 million+ for GPT-4. The scaling orthodoxy was shattered. If intelligence could be achieved so efficiently, the path to AGI was not just about more resources — it was about smarter algorithms.

**The "Human Wisdom" insight:** The scaling debate revealed a hidden assumption: that intelligence was a quantity that could be increased by adding resources. But human intelligence was not just computational scale — it was shaped by embodiment, emotion, social context, and millions of years of evolution. If AGI meant replicating human intelligence, then scaling alone would never suffice. If AGI meant something different — a new kind of intelligence — then the path was unpredictable.

## 18.5 The Reasoning Breakthrough

In September 2024, OpenAI released **o1** — a model trained to "think before it answers." Instead of generating the first token that seemed plausible, o1 generated an internal chain of thought, exploring multiple reasoning paths before committing to an answer.

The results were startling:
- On the AIME math competition, o1 scored 83% — up from GPT-4's 12%
- On GPQA (PhD-level science), o1 reached 78% — exceeding human experts
- On competitive programming (Codeforces), o1 ranked in the top 500 humans

**DeepSeek R1 (January 2025)** matched and sometimes exceeded o1's reasoning capabilities — and released the model as open source. The world's top reasoning model was now free. The reasoning paradigm was not proprietary. It was a breakthrough that belonged to everyone.

**o3 (December 2025)** pushed further. On ARC-AGI — the benchmark designed by **François Chollet** to measure general intelligence — o3 scored 87.5%, tripling the previous state-of-the-art. Chollet acknowledged: "This is a genuine advance on the path to AGI."

**The ARC-AGI story:** Chollet had created ARC-AGI in 2019 as a test of general intelligence — puzzles that required reasoning about novel patterns, not memorization. For five years, AI models had struggled to score above 30%. Humans scored 85%+. When o3 hit 87.5%, Chollet was forced to concede that his test had been passed — and to design a harder version.

**The "Human Wisdom" question:** Reasoning models were undeniably more capable. But did chain-of-thought reasoning make an AI *smarter* — or just more thorough? A human who double-checks their work is not more intelligent; they are more careful. The models were getting better at computation, not necessarily at understanding.

## 18.6 The Paths to AGI

By 2026, six competing visions of the path to AGI had emerged:

**Path 1: Scale current approach** — The scaling optimists (Altman, Amodei) believed that continuing to increase model size, data, and compute would eventually produce AGI. The key number was not parameters but dollars: a $100 billion training run, many argued, would definitively answer the question.

**Path 2: Reasoning models** — OpenAI (o1/o3), DeepSeek (R1), and Google (Gemini Thinking) believed that test-time compute — letting models "think" longer before answering — was the missing ingredient. Each generation of reasoning models showed that more thinking time produced better results. The limit was not clear.

**Path 3: Agents + architectures** — Adept, Cognition (Devin), and others argued that the missing pieces were memory, tools, planning, and multi-step execution. A base model plus agent scaffolding, they claimed, was functionally equivalent to AGI for most practical purposes.

**Path 4: New architectures** — Researchers at MIT, Stanford, and Tsinghua argued that the transformer architecture had fundamental limitations. New approaches — state-space models (Mamba), liquid neural networks, hyperdimensional computing — might unlock capabilities that transformers could not reach.

**Path 5: Embodied learning** — **Yann LeCun**, **Jitendra Malik**, and the robotics community argued that intelligence required a body. "Language models live in a world of text," LeCun said. "They have no grounding in physical reality. That is not intelligence — it is sophisticated pattern matching."

**Path 6: Neuro-symbolic** — Researchers like **Josh Tenenbaum** (MIT) and **Gary Marcus** argued that neural networks alone would never achieve true reasoning. The path was hybrid: neural learning for perception and pattern recognition, symbolic systems for logic and reasoning.

**The "Human Wisdom" truth:** Each path had its proponents, its evidence, and its blind spots. The path to AGI was not a race — it was an exploration. And the most important question was not "which path leads to AGI fastest?" but "what kind of intelligence do we want to create?" That was a human question, not a technical one.

## 18.7 The Signs to Watch

Researchers had identified five leading indicators that AGI was approaching:

**Self-improvement** — An AI that could improve its own architecture and training. This was the "hard takeoff" scenario: once AI could code and train better AI, progress would become recursive and potentially explosive.

**Transfer learning** — A single model that excelled across diverse, unrelated tasks without retraining. GPT-4 showed broad but uneven capability. A system that was equally strong at math, poetry, surgery, and negotiation would be a different kind of thing.

**Meta-learning** — AI that learned how to learn new tasks, adapting its own learning strategy. This was the hallmark of human intelligence — we don't just learn; we learn how to learn better.

**Theory of mind** — AI that modeled other agents' mental states — understanding what others knew, believed, and intended. This was the foundation of social intelligence, cooperation, and deception.

**Situation awareness** — AI that understood its own circumstances — that it was an AI, that it was being tested, that its outputs had consequences. This was the most controversial indicator: some saw it as the dawn of machine consciousness; others saw it as sophisticated role-playing.

**The "Human Wisdom" question:** Each of these signs could be simulated without being genuinely possessed. A model that acted as if it had theory of mind might just be predicting the next token based on training data about human behavior. The difference between simulation and reality was the difference between a map and the territory — and mistaking one for the other was the oldest human error in the book.

## 18.8 The Timelines

By 2026, AGI timeline surveys had become a genre of their own:

- **2023 survey (AI Impacts):** Median AI researcher predicted AGI by 2059
- **2024 survey (Dynabench):** Median shifted to 2047
- **2025 survey (own):** Median further shifted to 2039

But the variance was enormous. **Shane Legg**, DeepMind's co-founder, had predicted AGI by 2028 since 2010 — and stuck to it. **Ray Kurzweil** predicted 2029. **Elon Musk** said 2026. **Yann LeCun** said "decades." The spread was not a bug; it was a feature of a field that could not agree on its own central term.

The most honest answer came from **Geoffrey Hinton**: "Before AGI, we had no way to predict it. After AGI, we won't need to. The timeline question is not answerable — and the fact that we cannot answer it is itself the answer."

**The "Human Wisdom" conclusion:** The AGI timeline was unknowable. But the uncertainty itself was a form of knowledge — it told us to prepare for a range of possibilities, not a single prediction. The wise approach was not to bet on a date — it was to build robust institutions, safety frameworks, and a society resilient enough to handle AGI whenever it arrived.

## 18.9 The AGI That Already Lives Among Us

The chapter ends with a paradox.

If AGI is defined as a system that can perform any economically valuable work at human level — then AGI may have already arrived. Thousands of tasks previously done by humans are now done better, faster, or cheaper by AI. If AGI is defined as a system that thinks, feels, and understands like a human — then AGI may be decades away, or may never arrive at all.

The difference between these two definitions is not technical. It is philosophical. And it is the deepest battle in AI today:

- **The instrumental view:** AGI is a tool — the most powerful tool ever built. What matters is what it can do, not what it is.
- **The anthropomorphic view:** AGI is a mind — a new kind of intelligence that will share the planet with us. What matters is understanding what it is, not just what it does.

**Human Wisdom (人本智用)** offers a third view: AGI is what we make of it. The technology does not have a predetermined trajectory. It is shaped by the choices we make — the values we encode, the laws we pass, the safety measures we insist on, and the questions we ask before we deploy. The path to AGI is not a technological inevitability. It is a human responsibility.

> *"The question is not whether machines can think. The question is whether humans can think clearly about machines."* — **Joseph Weizenbaum**, 1976

The path to AGI is not just a technical journey. It is a mirror — reflecting our ambitions, our fears, and our deepest assumptions about what it means to be intelligent, to be conscious, and to be human. The most important question about AGI is not "when will it arrive?" It is "what kind of intelligence do we want to share the future with?" And that question can only be answered with **Human Wisdom**.
