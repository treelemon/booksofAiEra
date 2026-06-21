# 附录 A：关键基准测试解读

| 基准测试 | 衡量内容 | 2026 年饱和程度 | 参考链接 |
|----------|----------|----------------|----------|
| **MMLU** | 跨 57 个学科的多任务语言理解 | ~96% | [论文](https://arxiv.org/abs/2009.03300) |
| **GSM8K** | 小学数学应用题 | ~98% | [论文](https://arxiv.org/abs/2110.14168) |
| **MATH** | 竞赛数学 | ~94% | [论文](https://arxiv.org/abs/2103.03874) |
| **SWE-bench Verified** | 真实世界 GitHub 问题解决 | ~97% | [官网](https://www.swebench.com/) |
| **HumanEval** | 从文档字符串生成 Python 代码 | ~95%+ | [GitHub](https://github.com/openai/human-eval) |
| **BIG-Bench** | 204 个多样化任务（推理、逻辑、常识） | 混合 | [论文](https://arxiv.org/abs/2206.04615) |
| **HellaSwag** | 常识推理（句子补全） | ~95% | [论文](https://arxiv.org/abs/1905.07830) |
| **TruthfulQA** | 真实性和避免常见误解 | ~70% | [论文](https://arxiv.org/abs/2109.07958) |
| **MMMU** | 多模态理解（大学水平） | ~89% | [官网](https://mmmu-benchmark.github.io/) |
| **MathVista** | 视觉数学推理 | ~82% | [官网](https://mathvista.github.io/) |
| **OSWorld** | 智能体完成真实计算机任务 | ~66% | [论文](https://arxiv.org/abs/2404.07972) |
| **Chatbot Arena** | 人类偏好排名（ELO） | 无上限 | [排行榜](https://lmarena.ai/) |

**关键洞见：** 大多数基准测试正在饱和。需要新的、更难的基准来跟踪持续进展。
