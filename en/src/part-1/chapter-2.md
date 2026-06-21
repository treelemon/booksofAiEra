# Chapter 2: The Transformer Revolution

## 2.1 Before Transformers

Before 2017, sequence modeling meant RNNs, LSTMs, and GRUs — processing tokens one at a time. This was slow, hard to parallelize, and struggled with long-range dependencies.

## 2.2 "Attention Is All You Need" (2017)

The Vaswani et al. paper introduced the Transformer architecture. The core innovation: **the attention mechanism** lets every token look at every other token directly, regardless of distance.

**Key components:**
- **Self-attention:** each token attends to all others, weighted by relevance
- **Multi-head attention:** multiple attention patterns in parallel
- **Positional encoding:** gives the model a sense of token order (since attention is permutation-invariant)
- **Encoder-decoder stack:** original architecture; modern LLMs use decoder-only

## 2.3 Scaling Laws

Kaplan et al. (2020) and later Chinchilla (2022) showed that model performance follows predictable power-law relationships with:
- **Parameter count** (bigger models)
- **Data size** (more tokens)
- **Compute budget** (more FLOPs)

The practical implication: throwing more compute at a well-trained transformer predictably improves performance. This discovery triggered the scaling race.

## 2.4 Emergent Abilities

At certain scale thresholds, models suddenly display capabilities they weren't explicitly trained for:
- In-context learning (GPT-3)
- Chain-of-thought reasoning (PaLM, GPT-4)
- Instruction following (InstructGPT/ChatGPT)
- Code generation, translation, tool use

Not everyone agrees emergence is real — some argue it's a measurement artifact — but either way, bigger models *feel* qualitatively different.

## 2.5 The Post-Transformer Landscape

Transformers are no longer the only game:
- **Mamba, RWKV:** state-space models with linear-time inference
- **Hybrid architectures:** combining transformers with SSMs or MoE layers
- **DeepSeek's MoE:** Mixture-of-Experts for efficient scaling

But the core insight — attention-based architectures that scale with data and compute — remains the foundation of everything that follows.
