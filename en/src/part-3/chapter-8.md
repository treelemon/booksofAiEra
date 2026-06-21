# Chapter 8: Multimodal and Embodied AI

## 8.1 The "Her" Moment: GPT-4o Changes Everything

On May 13, 2024, **Mira Murati** — OpenAI's CTO at the time — stood on a stage in San Francisco and demonstrated something that felt like science fiction. GPT-4o ("omni") could see, hear, and speak in real time. It could read your facial expressions, detect your emotional state, and respond with natural intonation, laughter, and pauses.

The demo that went viral: Mira asked the model to tell a bedtime story in an increasingly dramatic voice. GPT-4o went from calm narrator to dramatic performer, complete with tension, whispers, and a roaring finale. It felt like talking to a person — or like **Scarlett Johansson's AI character in the film *Her***.

The comparison was so powerful that OpenAI accidentally hired an actor whose voice sounded like Johansson, leading to a controversy that forced OpenAI to pause the voice feature. But the genie was out of the bottle: AI had crossed the multimodal Rubicon.

GPT-4o processed **text, images, audio, and video** natively — a single neural network trained on all modalities simultaneously. Previous approaches had stitched separate models together. GPT-4o was one model, trained end-to-end on everything. The latency for voice conversations dropped from 5 seconds (GPT-4 + Whisper + TTS pipeline) to 320 milliseconds — indistinguishable from human conversation.

## 8.2 Sora: The World Simulator

Three months earlier, in February 2024, OpenAI had released another bombshell: **Sora**, a text-to-video model that could generate photorealistic 60-second videos from a sentence.

The demos were hypnotic. A woman walking through Tokyo at golden hour — rain on the pavement, reflections, consistent lighting. A woolly mammoth in the snow — fur moving naturally, snowflakes settling. A cat waking up in bed — the sheets moved like real sheets.

The research paper described Sora not as a video model but as a **"world simulator"** — it had learned physics, lighting, object permanence, and cause-and-effect through video data. It could simulate a scene, not just render pixels.

The limitations emerged quickly: Sora struggled with complex multi-object interactions, often making objects disappear and reappear. It was bad at cause-and-effect — a character might pour coffee into a cup and the cup would remain empty. It was a world simulator with no guaranteed consistency.

By 2026, Sora had been superseded by **OpenAI's Sora 2**, Google's **Veo 3**, and China's **Kling 2.0** — each capable of 2-minute photorealistic videos with significantly better consistency. The gap between Sora 2024 and Sora 2026 was larger than the gap between the first iPhone and the iPhone 14.

## 8.3 The Gemini Thesis: Born Multimodal

**Demis Hassabis**, CEO of Google DeepMind, had argued since 2023 that multimodality was not a feature — it was the path to general intelligence. "Human intelligence is deeply multimodal," he told the MIT Technology Review. "We learn by seeing, hearing, touching. An AI that only processes text is missing most of the world."

Google's execution of this thesis was methodical. **Gemini** was trained from the ground up as a multimodal model — not text-first with vision bolted on. The result: Gemini Ultra (December 2023) was the first model to beat GPT-4 on MMLU. By Gemini 2.5 Pro (2025), the model could natively process 1 million tokens of text, images, audio, and video — and reason across them in a single pass.

Google's unique advantage was data: YouTube (billions of hours of video), Google Images (hundreds of billions of photos), Google Earth (trillions of spatial data points), and Google's audio corpus (Google Voice, Google Meet, YouTube audio). No other company had access to this scale of multimodal data.

The result was a model that could watch a 10-hour video lecture, analyze the slides, read the cited papers, and answer questions about the content. By 2026, Gemini 3 Ultra had become the default choice for scientific research — not because it was the smartest model, but because it could ingest the most data.

## 8.4 The Robot Awakening

While language models dominated headlines, a parallel revolution was happening in hardware.

**Tesla Optimus (Elon Musk):** In 2024, Optimus could pick up objects from a table — slowly, carefully, like a toddler learning to grab. By 2026, Optimus Gen 3 could fold laundry, sort parts on an assembly line, and navigate uneven terrain. Musk's bet: "Optimus will be bigger than Tesla's car business." The skeptics noted that the timeline had slipped three times, but the progress was real.

**Figure 02 (Brett Adcock):** Figure Robotics partnered with OpenAI to put GPT-4's reasoning into a humanoid body. In 2024, a viral demo showed Figure 02 talking to a human: "What do you see?" — "I see a red apple on a plate." — "Can you hand it to me?" — The robot picked up the apple and handed it over. The demo was teleoperated for some movements, but the reasoning was real. By 2026, Figure 02 could work autonomously in a BMW factory for 8-hour shifts.

**Physical Intelligence (π0, 2024):** A startup founded by **Chelsea Finn** (Stanford) and **Sergey Levine** (UC Berkeley) released π0 — a vision-language-action model trained on internet data and robot data. The demo: π0 watched a human fold laundry once, then folded laundry itself. The generalization was the breakthrough — one model could fold clothes, load a dishwasher, and make coffee.

The common theme: **foundation models in robot bodies.** The same scaling laws that drove GPT-3's emergence were being applied to physical tasks. The hardware was still expensive ($150K per Optimus unit), but the software was learning faster than anyone expected.

**The embodied AI landscape by 2026:**

| Company / Lab | Robot | AI Approach | Best Capability | Status |
|--------------|-------|-------------|-----------------|--------|
| Tesla | Optimus Gen 3 | End-to-end neural net from video | Assembly line sorting, laundry folding, uneven terrain | Early production (~1,000 units) |
| Figure Robotics | Figure 02 | GPT-4 reasoning + teleoperation fine-tuning | BMW factory 8-hour autonomous shifts | Production deployment |
| Physical Intelligence | π0 | Vision-language-action model, one model many tasks | Generalization — fold clothes, load dishwasher, make coffee | Research stage |
| Google DeepMind | RT-2 / AutoRT | Trained on internet + robot data | Zero-shot generalization to new tasks | Research stage |
| Meta | Sparrow + Habitat simulator | Sim-to-real transfer | Manipulation in simulated environments | Research stage |

The key divide: Tesla and Figure were building specific hardware platforms with increasingly capable AI brains. Physical Intelligence was building a general-purpose AI brain that could work on any robot. The former was a hardware race; the latter was a software race. History suggests the software race will matter more.

## 8.5 The Multimodal Frontier

By 2026, the standard for "multimodal" had escalated dramatically:

| Capability | 2023 | 2026 |
|-----------|------|------|
| Image recognition | Classify objects | Describe composition, lighting, intent |
| Video understanding | Clip-level | Full-narrative reasoning |
| Audio processing | Speech-to-text | Emotion, speaker ID, sound event detection |
| Video generation | 4 second clips | 2 minute coherent scenes |
| Real-time voice | 5 second latency | 320ms with emotion |

The benchmark leaderboard told the same story: MMMU (multimodal reasoning) had gone from 60% to 89%. MathVista (visual math) from 45% to 82%. Video-MME (video understanding) from 55% to 76%.

## 8.6 The Apple Strategy: Edge Multimodality

**Tim Cook's** Apple took a different path: instead of building the biggest cloud model, Apple built the best on-device AI.

Apple Intelligence (announced June 2024, launched September 2024) brought multimodality to the device in your pocket. The **A18 Pro** and **M4** chips included a 16-core Neural Engine capable of 38 trillion operations per second — enough to run a 30-billion-parameter model locally.

The capabilities: real-time notification prioritization, image generation (Image Playground), custom emoji (Genmoji), on-device writing assistant, and Siri with screen awareness — you could ask "what time is my next meeting?" and Siri could see the calendar on your screen.

The privacy message was Apple's differentiator: "AI that understands you without collecting you." By 2026, Apple Intelligence was processing over 1 billion on-device requests per day. Samsung's Galaxy AI and Google's Pixel AI followed the same trajectory — powerful AI running locally, with cloud fallback for complex tasks.

## 8.7 The Embodiment Question

A debate simmered beneath the multimodal progress: **is embodiment necessary for intelligence?**

**Yann LeCun** (Meta's chief AI scientist) argued yes: "Intelligence emerges from interaction with the physical world. You can't be smart if you've never touched anything." Meta was investing heavily in embodied AI — PyRobot, Habitat simulator, and partnership with robotics labs.

**Andrew Ng** (DeepLearning.AI) argued the opposite: "Language contains enough of the world's structure. You can learn physics from text. You can learn causality from text. Embodiment helps, but it's optional."

The evidence by 2026 was mixed. Multimodal models that processed video of physical tasks learned some physics — object permanence, gravity, collision — without embodiment. But they struggled with properties that required interaction — weight, texture, rigidity. A model could watch a thousand videos of someone picking up a box, but it would not know whether the box was heavy or light until it lifted it.

The unresolved question: **Will true understanding require a body?** The answer would determine whether AI remains a software technology — or becomes a robotics technology.

**The embodiment debate framework:**

| Position | Proponents | Argument | Evidence | Implication |
|----------|-----------|----------|----------|-------------|
| Embodiment required | Yann LeCun, Meta | Intelligence emerges from physical interaction; language alone is insufficient | Multimodal models still struggle with weight, texture, rigidity — properties requiring touch | AI will need robotics; software-only path is limited |
| Embodiment optional | Andrew Ng, DeepLearning.AI | Language contains enough structure to learn physics and causality | Models can pass physics benchmarks, understand object permanence from video alone | AI can reach AGI without a body |
| Hybrid position | Demis Hassabis, DeepMind | Embodiment helps but may not be necessary; simulation may be sufficient | Simulated robots in virtual environments learn complex tasks; transfer to reality improving | Simulation may bridge the gap; physical embodiment optional |

The debate will resolve not through argument but through engineering. If a software-only model achieves AGI-level reasoning on embodied tasks without a body, LeCun is wrong. If the most capable systems consistently require physical training data, Ng is wrong. The 2026 evidence leans toward hybrid: embodiment helps, but simulation and video are narrowing the gap faster than expected.
