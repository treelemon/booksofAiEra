# Chapter 2: The Transformer Revolution

## 2.1 The Recurrent Prison

Imagine reading a sentence one word at a time — and having to hold every previous word in your head, in order, without ever looking back. That was the world before 2017.

RNNs, LSTMs, and GRUs processed sequences token by token, maintaining a hidden state that tried to compress everything seen so far into a fixed-size vector. For short sentences, it worked. But for long-range dependencies — the pronoun at the start of a paragraph whose referent appears three paragraphs later — the signal decayed into noise.

Training was equally painful. RNNs required sequential computation: you could not parallelize across time steps. Training GPT-1's 117-million-parameter RNN predecessor on a single corpus would have taken weeks. By 2017, the community knew something had to give.

Then eight Google researchers published a paper that would change the world.

## 2.2 The Eight Who Changed Everything

The author list of "Attention Is All You Need" reads like a founding myth: **Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Łukasz Kaiser, and Illia Polosukhin.** Eight people, from eight different backgrounds, brought together at Google by a shared conviction: the sequential bottleneck could be eliminated entirely.

The radical bet: throw away recurrence. No RNNs. No LSTMs. Only attention.

**Self-attention** let every token look directly at every other token, regardless of distance. A word at position 1 could attend to a word at position 1,000 with the same computational cost as attending to its immediate neighbor. The architecture could also be fully parallelized during training — suddenly, training time dropped from weeks to hours.

The paper was presented at NeurIPS 2017 and initially received with polite interest, not revolution. Few realized that this single architectural change — attention without recurrence — would unlock everything that followed.

## 2.3 The Road to Emergence: A Timeline of Surprises

The transformer did not arrive fully formed. It was a series of discoveries, each more surprising than the last:

**GPT-1 (June 2018, 117M parameters):** OpenAI demonstrated that a decoder-only transformer could learn language modeling and transfer to downstream tasks with minimal fine-tuning. The results were modest but the principle was powerful.

**BERT (October 2018, 340M parameters):** Google counter-punched with a bidirectional encoder. By masking words and asking the model to predict them, BERT achieved state-of-the-art on 11 NLP benchmarks. The encoder-decoder vs. decoder-only debate began.

**GPT-2 (February 2019, 1.5B parameters):** OpenAI scaled up. The results were so coherent that OpenAI initially withheld the full model, citing concerns about misuse. The "GPT-2 controversy" taught the world to pay attention to scaling.

**GPT-3 (May 2020, 175B parameters — 100× GPT-2):** This was the earthquake. At 175 billion parameters, trained on ~570GB of text, GPT-3 could perform tasks it had never been explicitly trained to do — translate languages, write code, answer questions — simply by seeing a few examples in the prompt. The phenomenon was named **in-context learning**, and nobody had predicted it. Ilya Sutskever later admitted the team was genuinely surprised.

**Chinchilla (March 2022):** DeepMind made a counterintuitive discovery: for a given compute budget, most models were undertrained. The optimal strategy was to train a smaller model on *far more data*. Chinchilla (70B parameters, 1.4 trillion tokens) outperformed GPT-3 (175B parameters, 300 billion tokens). The scaling race suddenly had a new rulebook.

**GPT-4 (March 2023):** Multimodal, more reliable, dramatically better at reasoning. OpenAI revealed few technical details but confirmed it used an MoE architecture. Eliezer Yudkowsky, after testing it, remarked: "This is strange and worrying... it's not yet smarter than a human, but it's smarter than most humans on most tasks."

## 2.4 Scaling Laws: The North Star

The empirical discovery that turbocharged the entire race came from Kaplan et al. (2020): model performance follows a smooth power-law relationship with three variables:

- **Model size** (parameters): doubling parameters predictably reduces loss
- **Dataset size** (tokens): doubling training data predictably reduces loss
- **Compute budget** (FLOPs): the total allocation determines the optimal trade-off

This was the North Star of the AI industry. It meant that throwing more compute at a well-trained transformer would predictably improve intelligence — no architectural breakthroughs required. It turned AI from a research problem into an engineering scaling problem.

The economic implication was dizzying: if you could afford a $100 million training run, you could buy a predictable improvement in model quality. The scaling race was on.

Chinchilla refined the picture in 2022: most models were compute-optimal for the wrong regime. The correct recipe was to scale data faster than parameters. This led directly to LLaMA (Meta, 2023), which trained a 65B model on 1.4 trillion tokens — disproving the notion that only the largest models could compete.

## 2.5 The Encoder-Decoder Fork and the Rise of Decoder-Only

A fork emerged in the transformer family tree:

- **Encoder-decoder (T5, BART):** bidirectional understanding + generative output. Strong for translation and summarization.
- **Decoder-only (GPT series, LLaMA, Claude, Gemini):** unidirectional, autoregressive. Dominant for general-purpose AI.

By 2024, decoder-only had won. The reasoning: language generation is inherently autoregressive, and the simplicity of a single stack scaled better. Every frontier model — GPT-4, Claude 3, Gemini, DeepSeek — used decoder-only transformers with minor variations.

## 2.6 The Post-Transformer Landscape

Transformers are no longer the only game, but every challenger measures itself against the architecture they dethroned:

- **Mamba (2024):** state-space model with linear-time inference. Matches transformers on long-context tasks while using 5× less memory.
- **RWKV (2024):** combines transformer-style attention with RNN-style linear-time inference.
- **Hybrids (2025):** Jamba (AI21), Samba (Microsoft), and others mix transformer layers with SSM or MoE layers for best-of-both-worlds performance.
- **DeepSeek's MoE (2024–2025):** mixture-of-experts architecture where only a fraction of parameters activate per token, enabling massive effective scale at lower cost. DeepSeek-V3 (671B total, 37B active) and DeepSeek-R1 showed that open-source models could match frontier performance through architectural cleverness.

The transformer's dominance is no longer unchallenged, but its core insight — attention-based architectures that scale predictably with data and compute — remains the foundation of the current AI era. Whatever comes next will be measured against the revolution that eight researchers sparked on a whiteboard at Google in 2017.
