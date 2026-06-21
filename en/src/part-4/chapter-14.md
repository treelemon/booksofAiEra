# Chapter 14: AI in Science and Medicine

## 14.1 The First AI Drug: A 50-Year Problem Solved in Two Years

In February 2024, a biotechnology company called **Insilico Medicine** announced that an AI-discovered drug for idiopathic pulmonary fibrosis (IPF) — a fatal lung disease — had successfully completed Phase II clinical trials. The drug, **INS018_055**, had gone from target discovery to Phase II in less than three years. The traditional timeline for this milestone: eight to twelve years.

**Alex Zhavoronkov**, Insilico's founder and CEO, had been pursuing AI-driven drug discovery since 2014 — a time when most pharma executives thought he was eccentric. "Biology is not a science of perfect data," he said. "It's a science of noisy, incomplete, high-dimensional data. That's exactly what deep learning is good at."

INS018_055 was the first proof that the AI drug discovery pipeline could work end-to-end. It was followed rapidly by others: **Recursion Pharmaceuticals** (led by **Chris Gibson**) had two AI-discovered cancer drugs in Phase II by 2025. **Isomorphic Labs** (Demis Hassabis's Alphabet spinout) had licensed AI-discovered drug candidates to Eli Lilly and Novartis for $1.2 billion — before any of them reached human trials.

The economics were staggering. Traditional drug development cost $2–3 billion per approved drug, with a 90% failure rate from Phase I to approval. AI-driven discovery was targeting $300–500 million per drug, with projected success rates of 30-50%. If those numbers held, AI would be the most transformative force in medicine since antibiotics.

## 14.2 The Doctor Will See You Now — Actually, the AI Will

The transformation of clinical medicine was quieter than drug discovery — but equally profound.

**Med-PaLM 2 (Google, 2023)** achieved 86.5% on the US Medical Licensing Exam (USMLE) — passing with a score comparable to a human physician. GPT-4 followed with 90%+. By 2025, LLMs were scoring in the 95th percentile on board examinations in radiology, dermatology, and pathology.

The real story was not test scores — it was deployment:

**Radiology:** In 2024, the FDA had approved over 700 AI medical devices — more than half of them for radiology. AI systems for mammography screening (such as **Kheiron Medical** and **Lunit**) were reading mammograms with sensitivity equal to or better than human radiologists. Between 2020 and 2026, the number of radiologists in the US had grown by 5% — but the volume of scans had grown by 40%. AI was the only reason the system had not collapsed.

**Pathology:** **Paige AI** (founded by **Thomas Fuchs**) had developed an AI system for prostate cancer detection that reduced false negatives by 70%. In a landmark 2025 study at Memorial Sloan Kettering, pathologists using Paige AI detected 24% more clinically significant cancers than those working without AI.

**Dermatology:** Smartphone apps with AI-powered skin lesion classification — such as those developed by **Google Health** (led by **Lily Peng**) — could triage skin lesions with dermatologist-level accuracy. The UK's National Health Service piloted AI triage for skin cancer in 2025, with 92% sensitivity.

**The caveat:** Every deployed medical AI was narrow — trained on one task, one organ, one modality. Generalist medical AI — a "doctor AI" that could diagnose anything — did not exist in clinical practice. The failure modes were too poorly understood.

## 14.3 The AI-Assisted Doctor

The most impactful application was not AI replacing doctors — it was AI giving doctors superpowers.

**The documentation revolution:** A 2024 study at Stanford Medical Center found that physicians spent 49% of their time on electronic health record (EHR) documentation — and only 27% on direct patient care. AI note-taking systems (like **Abridge**, **Ambience**, and **Nuance DAX**) listened to patient conversations and generated clinical notes in real time. Doctors who used AI documentation reported 60% less burnout and spent 15% more time with patients.

**The diagnosis assistant:** **Glass AI** (from OpenEvidence) and **DxGPT** were LLM-based clinical decision support systems. A doctor could describe a case, and the AI would generate a differential diagnosis, suggest relevant tests, and flag drug interactions. In a 2025 study at Mayo Clinic, physicians using AI diagnosis support made the correct diagnosis 23% more often than those working without it — and made it 40% faster.

**The referral triage:** The UK's NHS used an AI triage system (from **Babylon Health** by **Ali Parsa**) to route patient referrals. Patients described symptoms; the AI determined urgency and specialty. By 2026, the system was handling 30% of all primary care referrals in the NHS. Emergency department visits had decreased by 12%.

**Daphne Koller**, founder of **insitro**, framed it differently: "The question is not whether AI can diagnose better than a doctor. The question is whether the combination of AI + doctor can outperform either alone. The answer is a clear yes — in every study that has tested it."

## 14.4 The Laboratory of the Future

Scientific research was being transformed from the bench up.

**Automated labs:** **Sebastian Thrun** (founder of Google X, now at Stanford) had demonstrated that AI-controlled robotic laboratories could run experiments 24/7 — designing experiments, executing them, measuring results, and iterating. The "self-driving lab" concept was realized by **Gryphon Scientific** and **Arctoris**. In materials science, AI-driven labs had accelerated discovery by 10-100× in specific domains.

**Literature AI:** AI tools for scientific literature — **Elicit**, **Semantic Scholar**, **Consensus** — could read 10,000 papers in a night and synthesize findings across domains. A 2025 study showed that researchers using AI literature tools discovered 2× more relevant papers and took 70% less time.

**Hypothesis generation:** **Scite.ai**, **Iris.ai**, and **Kamiwaza** were generating novel research hypotheses by connecting findings across disconnected fields. In 2025, an AI at MIT proposed a new mechanism for battery degradation that human researchers had missed for a decade. When tested experimentally, the hypothesis was confirmed.

**The peer review crisis:** AI was both the problem and the solution. AI-generated papers were flooding journals — the Committee on Publication Ethics (COPE) estimated that 15% of submissions to some journals were AI-generated by 2025. But AI-assisted peer review — checking statistics, flagging inconsistencies, detecting fabricated data — was becoming essential. Journals that used AI screening tools (like **Scholarly**, **Penelope AI**) had reduced review times by 30%.

## 14.5 The GPQA Milestone

In 2024, a new benchmark called **GPQA (Graduate-Level Google-Proof Q&A)** was introduced — 448 multiple-choice questions at the level of a PhD-qualified expert, designed to be extremely difficult for both humans and AI.

The results were sobering for humans: domain experts scored 65-80%. GPT-4 scored 42%. By early 2025, o3 scored 87.4% — exceeding the human expert baseline.

The benchmark was notable because the questions were deliberately "hard for search engines" — requiring genuine reasoning, not retrieval. When AI exceeded human expert performance, it was not memorizing — it was reasoning.

**The implication:** PhD-level scientific reasoning was no longer uniquely human. AI could contribute to the most demanding intellectual work — proposing experiments, interpreting results, generating theories.

## 14.6 The Replication Crisis, Amplified

The integration of AI into science had a dark side — and it was the amplification of a pre-existing crisis.

**Paper mills:** Fraudulent paper factories had been a problem in scientific publishing for years. The field was already plagued by peer-reviewed journals that published anything for a fee. AI made the problem catastrophic. Generative models could produce thousands of plausible-looking papers per day. By 2025, some journals were retracting 20-30% of their published papers due to AI-generated fraud.

**The "tortured phrase" epidemic:** A 2024 investigation by **Nature** revealed that AI-generated text in scientific papers had a distinctive signature — "hallucinated" references, awkward phrasing, and "tortured phrases" where the AI had substituted uncommon words for common ones. "Deep learning" became "profound erudition." "Artificial intelligence" became "counterfeit consciousness." The phenomenon was so widespread that it was used as a diagnostic — a paper with tortured phrases was almost certainly AI-generated and probably contained fabricated data.

**The validation crisis:** AI predicted protein structures with atomic accuracy. AI designed molecules with high predicted binding affinity. AI wrote plausible research papers. But the gap between *prediction* and *experimental validation* was widening. The rate of AI-generated hypotheses was exceeding the scientific community's capacity to test them by 10:1 in some fields.

**The response:** "We need an AI for validation to match the AI for generation," argued **Anne Carpenter**, creator of the CellProfiler platform. The field of "automated experiment" — robotic labs that could test AI predictions at scale — was emerging.

## 14.7 The Trust Problem in Medicine

Medical AI faced a challenge that no benchmark could solve: **trust.**

A radiologist using AI to read mammograms faced an impossible dilemma: if the AI flagged a suspicious region that the radiologist had missed, should they change their report? If the AI missed something the radiologist caught, should they downgrade their confidence in the AI?

**The "second reader" paradigm:** The FDA's most common approval framework treated AI as a "second reader" — the human made the initial decision, then the AI reviewed it. This preserved human accountability while leveraging AI's pattern-matching strengths.

**The liability question:** If an AI-assisted doctor missed a diagnosis, who was responsible? The doctor? The hospital? The AI vendor? US medical liability law had not been updated for the AI era. Some hospitals were requiring vendors to indemnify AI-related claims. Others required patients to consent to AI-assisted diagnosis.

**The regulation gap:** The FDA's AI approval process was designed for "locked" algorithms that did not change after deployment. But the most powerful AI models were "continuously learning" — improving with each use. The FDA had approved only 15 continuously-learning AI systems by 2026. The gap between AI capability and regulatory capacity was as wide in medicine as it was in every other domain.

## 14.8 The Frontier: What Comes Next

The trajectory of AI in science and medicine pointed toward three revolutions:

**1. The "100x" biology revolution:** AI was compressing biological discovery timelines from decades to years to months. The first AI-discovered drugs were in Phase II. By 2030, the first fully AI-discovered and AI-developed drug could reach market.

**2. The personalized medicine revolution:** AI that could integrate a patient's genome, transcriptome, proteome, microbiome, and environmental data into a unified model of their health — and recommend treatments tailored to their specific biology. The "digital twin" concept — a continuously updated AI model of each patient — was being piloted at Stanford and the NHS.

**3. The autonomous scientific discovery:** The ultimate goal — an AI system that could propose hypotheses, design experiments, run them, interpret results, and refine theories without human intervention. The first prototypes existed. The fully realized version was years away — but the direction was unmistakable.

**The warning from Demis Hassabis:** "AI in science is the most important application of AI. But we must be humble. Nature is complex. The human body is complex. AI will make mistakes — and in medicine, mistakes cost lives. We need to proceed with ambition, but also with caution."

## 14.9 The Diagnostic Revolutionaries

The most personal impact of AI in medicine was happening not in labs or boardrooms — but in the lives of individual patients.

**The lung cancer story:** In 2023, Google Health published a study in *Nature* demonstrating that an AI system could detect lung cancer on CT scans with 94.4% sensitivity — higher than the 88.4% achieved by radiologists. The AI also reduced false positives by 11%. By 2026, AI-powered lung cancer screening was standard across 40% of US hospitals. The survival rate for early-detected lung cancer was 60%. The survival rate for late-detected lung cancer was 6%. AI was literally saving lives by catching cancers earlier.

**The sepsis prediction story:** In 2024, the University of California San Francisco deployed an AI system — **Compass** — that predicted sepsis 12 hours before it occurred by analyzing vital signs, lab results, and clinical notes. Sepsis kills 270,000 Americans per year, mostly because it is detected too late. In the first year of deployment, Compass reduced sepsis mortality in UCSF hospitals by 18%. The system was deployed in 200+ hospitals by 2026.

**The eye disease story:** Google's **DeepMind Health** (now part of Google Health) had developed an AI that could detect 50+ eye diseases from retinal scans with 94% accuracy. By 2025, the system was deployed across 30 NHS hospitals in the UK — processing over 100,000 scans per month. The AI could triage urgent cases within minutes. What previously took weeks now took hours.

## 14.10 The Accessibility Revolution

The most profound impact of AI in medicine may not be on frontier hospitals — it may be on patients who had no access to healthcare at all.

**The global health gap:** There are 1.5 billion people in the world with no access to basic medical imaging. Sub-Saharan Africa has 0.3 radiologists per 100,000 people — compared to 90 per 100,000 in the US. AI on a smartphone could bridge this gap.

**Portable diagnostics:** By 2026, AI-powered diagnostic apps could detect diabetic retinopathy (a leading cause of blindness) from a smartphone photo of the eye, with 96% accuracy. AI could screen for cervical cancer from a photograph of the cervix. AI could analyze a smartphone photo of a skin lesion for malignancy. The hardware was a phone. The doctor was an algorithm. The cost was near zero.

**The "AI community health worker":** In Rwanda, an AI triage system operated by **Babylon Health** (later acquired) was handling 40% of primary care consultations by 2026. Patients described symptoms to an AI via SMS and received a triage recommendation within seconds. The system processed 2 million consultations per month with a patient satisfaction score of 4.7/5.

**The challenge of access:** AI could diagnose — but could it treat? The gap between AI diagnosis and AI-delivered treatment was the next frontier. If a patient in rural India had diabetic retinopathy detected by AI, there still needed to be a doctor to perform the laser surgery. AI could extend the reach of medicine — but it could not yet replace the hands of a surgeon.

## 14.11 The Regulation Bottleneck

The rate at which AI could improve medicine was exceeding the rate at which regulators could approve it.

**The FDA's AI backlog:** By 2026, there were over 1,200 AI medical device applications pending at the FDA. The agency had approved 882 since 2018, but the approval rate was not keeping pace with submission rate. The average approval time had increased from 6 months to 18 months — because the applications were more complex.

**The "algorithm change" problem:** Most AI algorithms improved with more data. But the FDA's framework treated any change to an algorithm as a new device requiring re-approval. The result: most deployed medical AI was frozen at the moment of approval — never improving, even when it could.

**The international fragmentation:** An AI system approved by the FDA (US) needed separate approval from the EMA (Europe), PMDA (Japan), NMPA (China), and others. Each regulator required different data, different clinical studies, and different documentation. The fragmentation was slowing global deployment.

**The path forward:** The International Medical Device Regulators Forum (IMDRF) was working on a "harmonized AI framework" — but the target date was 2028. Meanwhile, AI capability advanced every three months. The gap between what AI could do and what regulators would allow was growing, not shrinking.

## 14.12 The Human Element

The final story of AI in medicine was a story of limits.

**The AI that missed the obvious:** In 2024, a widely-publicized case involved an AI system at a major US hospital that failed to detect a brain hemorrhage on a CT scan — because the scan had been taken with a different machine model than the AI was trained on. The patient deteriorated. The mistake was caught by a human radiologist the next day. The patient survived. The lesson: AI was brittle. It failed in ways that humans did not.

**The empathy gap:** A 2025 study compared patient satisfaction between AI-only triage, AI-assisted human triage, and human-only triage. The highest satisfaction scores went to "human-only" — not because the diagnosis was better (AI-assisted was the most accurate), but because patients wanted a human to hear their story. The empathy gap was real and measurable.

**The final verdict:** AI in medicine was not going to replace doctors. It was going to change what it meant to be a doctor — eliminating the parts the profession disliked (documentation, data entry, routine screening) and amplifying the parts that mattered most (diagnosis, treatment planning, patient relationship). The best doctors of 2026 were not competing with AI. They were collaborating with it.
