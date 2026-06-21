# Chapter 5: The Infrastructure Race

## 5.1 Compute as the New Oil

AI capability is compute-limited. Every frontier model requires:
- **Training:** tens of thousands of GPUs for months (hundreds of millions of dollars)
- **Inference:** massive serving infrastructure

The Stargate project (US, announced 2025) pledged $500B for AI infrastructure. The UK and Canada announced national compute initiatives. NAIRR (National AI Research Resource) provides academic access.

## 5.2 The Hardware Landscape

| Hardware | Strengths | Best For |
|----------|-----------|----------|
| NVIDIA H100/B200 | General purpose, software ecosystem | Training + inference |
| AMD MI350 | Competitive performance, lower cost | Inference |
| Google TPU v7 | Custom for TensorFlow/JAX | Training |
| AWS Trainium 3 | AWS integration | Training |
| ASIC accelerators | Task-specific efficiency | Inference |
| Chiplet designs | Modular, scalable | Edge + data center |
| Analog inference | Ultra-low power | Edge AI |
| Quantum-assisted | Emerging | Optimization |

## 5.3 The Efficiency Shift

The dominant narrative for 2025–2026 is **efficiency**, not raw scale:

- DeepSeek proved frontier performance at 10–20% of the cost
- MoE architectures reduce active parameters per token
- Quantization, distillation, pruning becoming standard
- Hardware-aware model design (co-optimization)

**Consequence:** The "scaling is all you need" era is over. Now we optimize.

## 5.4 Edge AI

In 2026, edge AI moves from hype to reality:
- On-device LLMs (Apple Intelligence, Samsung Galaxy AI)
- Specialized edge chips for agentic workloads
- Privacy-preserving local inference

**Implication:** AI capability will be ubiquitously available, not locked in data centers.

## 5.5 Geopolitics of Compute

Compute access is now a national security concern:
- US export controls on advanced chips to China
- China's domestically produced alternatives (Huawei Ascend)
- "Compute sovereignty" movements in Europe, India, Southeast Asia
- Open-source models as a workaround for compute-restricted regions
