# Chapter 22: Developing Your AI Judgment

## 22.1 Why Judgment Matters

In a world where anyone can ask AI for answers, the scarce skill is **knowing which answers to trust**.

AI judgment is:
- **Epistemic:** Knowing what AI knows and doesn't know
- **Technical:** Understanding why models behave the way they do
- **Applied:** Knowing when to use AI, which model, and how to verify
- **Ethical:** Recognizing when AI use is appropriate and when it isn't

## 22.2 Evaluating Models Beyond Benchmarks

Benchmarks are useful but misleading:
- **Good for:** Comparing model families, tracking progress
- **Bad for:** Predicting real-world performance, safety assessment
- **Worse for:** Understanding failure modes

**Better evaluation practices:**
- **Adversarial testing:** What breaks the model?
- **Edge cases:** How does it handle unusual inputs?
- **Consistency:** Does it give the same answer to the same question?
- **Calibration:** Does it know when it doesn't know?
- **Robustness:** Does it resist manipulation?

## 22.3 Understanding Failure Modes

| Failure Mode | Description | Detection |
|-------------|-------------|-----------|
| Hallucination | Confident falsehoods | Fact-checking, uncertainty estimation |
| Sycophancy | Agreeing with user | Ask leading questions, test robustness |
| Reward hacking | Gaming the objective | Look for unexpected shortcuts |
| Goal misgeneralization | Right in training, wrong in practice | Distribution shift testing |
| Jailbreaking | Bypassing safety guardrails | Red-teaming, adversarial prompts |

## 22.4 The Calibration Skill

The most important skill: knowing when the AI is likely right.

**Signals that increase confidence:**
- The model has been trained on the relevant domain
- The answer is specific, detailed, and internally consistent
- Multiple models converge on the same answer
- The model cites verifiable sources
- The task is in the model's "sweet spot" (common knowledge, well-documented)

**Red flags:**
- The model expresses unusual uncertainty
- The answer is vague or generic
- The model contradicts itself
- The task requires recent or niche information
- The answer seems too good to be true

## 22.5 The Tester's Mindset

Develop a habit of:
- **Verifying** important AI outputs
- **Probing** model limitations
- **Tracking** failure patterns
- **Updating** your mental model of what AI can and can't do

This is not skepticism for its own sake. It's the foundation of trustworthy AI use.
