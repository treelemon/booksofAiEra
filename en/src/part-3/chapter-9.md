# Chapter 9: AI for Discovery

## 9.1 The Nobel Prize That Changed Science

In October 2024, the Royal Swedish Academy of Sciences announced the Nobel Prize in Chemistry. The winners: **Demis Hassabis** and **John Jumper** of Google DeepMind, alongside **David Baker** of the University of Washington.

The prize was for protein folding — a problem that had haunted biology for 50 years. Proteins fold into three-dimensional shapes determined by their amino acid sequences. Get the shape, understand the function. For decades, determining a single protein structure cost hundreds of thousands of dollars and took years. By 2021, AlphaFold could predict the structure of any of the 200 million known proteins in minutes — for free.

The Nobel was not just for a scientific breakthrough. It was the moment the world recognized that AI had become a tool for *discovery*, not just automation.

## 9.2 AlphaFold: The Story Behind the Prize

**John Jumper** was a 35-year-old PhD who had left a career in physics to work on protein folding at DeepMind. In 2018, the first version of AlphaFold placed first in the biennial CASP competition — but the predictions were not accurate enough for practical use. Jumper and his team went back to the drawing board, rethinking the architecture from scratch.

**AlphaFold 2 (2020)** was the result. It achieved atomic-level accuracy — the equivalent of solving a 50-year-old grand challenge. The team published the code, the weights, and a database of 350,000 predicted protein structures. By 2025, over 2 million researchers worldwide had used AlphaFold. The database had expanded to cover all 200+ million known proteins.

**AlphaFold 3 (May 2024)** went further: it could predict interactions between proteins, DNA, RNA, and small molecules — opening drug discovery. For the first time, a computational model could simulate the molecular dance that underlies all of biology.

The impact was staggering. In 2023, researchers at the University of California used AlphaFold to identify a protein target for a new liver cancer drug — a process that traditionally took 5-10 years. They did it in 30 days.

## 9.3 AlphaEvolve: When AI Becomes the Inventor

In 2025, DeepMind released **AlphaEvolve** — and the definition of "AI capability" shifted again.

AlphaEvolve combined a large language model with evolutionary search to generate novel algorithms. The LLM proposed candidate algorithms; the evolutionary algorithm selected, mutated, and recombined the best ones; the cycle repeated. The result: algorithms for data center power management that reduced energy consumption by 15%, and TPU chip scheduling algorithms that improved throughput by 12%.

These were not optimizations of existing approaches. They were *new algorithms* — approaches that human engineers had never considered. When the DeepMind team analyzed the discovered solutions, they found strategies that were counterintuitive but effective.

**Max Jaderberg**, who led the AlphaEvolve team, described the moment: "We gave the system a problem, and it came back with something we hadn't thought of. Not a better version of our approach — a completely different approach."

Within weeks, the community had replicated and extended the work. **Asankhaya Sharma** released **OpenEvolve**, an open-source reproduction. Tokyo-based **Sakana AI** (founded by former Google researchers) released **SinkaEvolve**, adapting the approach for Japanese industrial problems. A US-China collaboration claimed improvements on AlphaEvolve's mathematical solutions.

The message was clear: AI could now invent. Not just retrieve or combine. *Invent*.

## 9.4 The Materials Revolution

Proteins were just the beginning. AI was rewriting the materials science playbook.

**GNoME (Graph Networks for Materials Exploration, 2023):** DeepMind's materials discovery model predicted 380,000 stable inorganic crystals — equivalent to 800 years of cumulative human discovery. The team synthesized 736 of the most promising candidates in a real lab and confirmed 41% were viable.

**MatterGen (Microsoft, 2024):** Microsoft's generative model for materials design could propose new materials with specific properties — a certain conductivity, a specific bandgap, a target tensile strength. By 2026, MatterGen had discovered a new battery cathode material that increased energy density by 27%.

**The carbon capture breakthrough:** In 2025, MIT researchers used AI to screen 10 million potential materials for carbon capture. The top candidate, a porous covalent organic framework, absorbed CO2 at 3× the rate of current best-in-class materials. The AI had discovered it in three weeks. Traditional methods would have taken 15 years.

**AI-for-discovery domains compared:**

| Domain | Breakthrough Model | Year | What It Achieved | Human-Equivalent Time | Impact |
|--------|-------------------|------|------------------|----------------------|--------|
| Protein folding | AlphaFold 2/3 | 2020/2024 | Predict 200M+ protein structures; simulate molecular interactions | Decades → minutes | Transformed structural biology; 2M+ researchers using it |
| Materials discovery | GNoME (DeepMind), MatterGen (Microsoft) | 2023/2024 | Predict 380K stable crystals; design materials with target properties | 800 years of discovery → months | Battery cathode with 27% higher energy density |
| Algorithm discovery | AlphaEvolve (DeepMind) | 2025 | Generate novel algorithms for datacenter power, chip scheduling | Human engineers never considered the solution | 15% energy reduction, 12% throughput gain |
| Mathematics | FunSearch, AlphaProof (DeepMind) | 2023/2024 | Solve cap set problem; earn IMO silver medal | Decades-stuck problem → solved | AI generates and verifies mathematical proofs |
| Drug discovery | AlphaFold 3, INS018_055 | 2024 | Identify drug targets in 30 days (vs 5-10 years); AI-discovered drug in clinical trials | 5-10 years → 30 days | AI-discovered molecule entered human trials |

The pattern: AI excels when the problem has a clear fitness function (fold this protein, maximize this crystal stability, minimize this energy), has accessible training data (known proteins, known materials, known algorithms), and can be verified in silico before physical validation.

## 9.5 The Automated Scientist

In August 2024, Sakana AI (founded by **Llion Jones** — a coauthor of "Attention Is All You Need") published a paper that made the research community uncomfortable.

**The AI Scientist** was a fully automated research system. It generated a research idea, wrote the code, ran the experiments, produced the figures, and wrote a paper with citations. The system cost $15 per paper — about 10,000× cheaper than the average academic paper.

The papers it produced were not Nobel-worthy. They were incremental improvements, minor findings — the kind that junior researchers and PhD students produce. But that was exactly the point. The AI Scientist was doing the *grunt work* of science.

The reaction was polarized:
- **Yoshua Bengio** warned: "Science is a human endeavor. Automating the creative process could cheapen discovery."
- **Andrew Ng** replied: "Science has always been about building tools that accelerate understanding. The AI Scientist is just the latest tool."
- **Llion Jones** responded: "We're not replacing scientists. We're giving them a research assistant that works 24/7, costs nothing, and never sleeps."

## 9.6 Mathematics: The Proof Machine

Mathematics proved to be a uniquely fertile ground for AI discovery.

**FunSearch (DeepMind, 2023):** An LLM combined with an automated evaluator discovered new solutions to the cap set problem — a combinatorial mathematics problem that had resisted progress for decades. The LLM proposed candidate mathematical constructions; the evaluator tested them; the best ones were fed back. The discovered construction was genuinely novel — no human mathematician had thought of it.

**AlphaProof (DeepMind, 2024):** A system that could generate and verify mathematical proofs. At the 2024 International Mathematical Olympiad, AlphaProof solved four out of six problems — earning a silver medal. It did not just solve the problems — it generated formal proofs that could be checked by a theorem prover.

**The implication:** Mathematics, long considered the most purely human intellectual activity, was no longer the exclusive domain of human creativity. AI was not just solving known problems — it was discovering new conjectures that no human had posed.

## 9.7 The Discovery Stack

By 2026, the pattern for AI-driven scientific discovery had converged on a common workflow:

1. **Hypothesis generation** — LLM proposes candidate solutions (molecules, algorithms, materials, mathematical constructions).
2. **Simulation** — The candidates are evaluated in silico (physics simulation, formal verification, protein folding prediction).
3. **Evolution** — An evolutionary algorithm or reinforcement learning loop iterates on the best candidates.
4. **Physical validation** — The most promising candidates are synthesized or tested in the real world (wet lab, prototype, deployment).
5. **Human interpretation** — Scientists analyze the AI's discoveries, extract principles, and design the next round of hypotheses.

The rate-limiting step had shifted. It used to be hypothesis generation — humans could only think of so many ideas. Now it was physical validation — there were only so many experiments a wet lab could run. The gap between *what AI could imagine* and *what science could test* was the new bottleneck.

## 9.8 The Frontier: Autonomous Discovery

The holy grail is a fully autonomous discovery machine — an AI that poses hypotheses, designs experiments, runs them, interprets results, and revises its theories.

We are not there yet. AlphaEvolve made a novel discovery — but within a well-defined search space. The AI Scientist produced papers — but on pre-selected problems. AlphaFold transformed biology — but protein structure prediction was a well-defined task.

The trillion-dollar question: **Can AI discover something truly fundamental — a new law of physics, a new mathematical foundation, a new principle of biology?**

**Demis Hassabis** believes the answer is yes: "We are at the beginning of the 'Century of Biology' and the 'Century of AI' simultaneously. The intersection is where the most important discoveries of the 21st century will come from."

**Yann LeCun** is more cautious: "Discovery requires understanding. Current AI systems don't understand anything. They are powerful pattern matchers, not scientists."

The trajectory favors Hassabis. Each year, AI discovery systems become more autonomous, more reliable, and more creative. The question is not *if* AI will make fundamental discoveries — it is *when*, and whether human science will be ready to accept them.

**The AI discovery maturity model:**

| Level | Description | Examples | Bottleneck |
|-------|-------------|----------|------------|
| L1: Assist | AI as tool for human scientists | AlphaFold predicting structures, LLMs for literature review | Human creativity |
| L2: Suggest | AI proposes candidates; human evaluates | GNoME proposing materials, FunSearch proposing math constructions | Physical validation capacity |
| L3: Optimize | AI iterates within defined search space | AlphaEvolve optimizing algorithms, AI Scientist writing papers | Problem definition |
| L4: Discover | AI finds genuinely novel solutions without human guidance | None yet (approached but not achieved) | Scientific creativity, ground truth |
| L5: Paradigm shift | AI discovers new laws of physics, new mathematical foundations | Speculative | Unknown — would require AI to challenge human conceptual frameworks |

We are at L2-L3 across most domains. L4 is on the horizon. L5 remains the trillion-dollar question. The rate of progress suggests L4 will arrive within 5-7 years — and L5 within 15-20, or not at all.
