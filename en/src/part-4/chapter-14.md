# Chapter 14: AI in Science and Medicine

## 14.1 The AI Capability Taxonomy in Scientific Domains

AI's contribution to science spans a spectrum from pattern recognition to autonomous hypothesis generation. Understanding where AI excels, where it augments, and where it falls short is essential for researchers and clinicians.

**Scientific capability domain matrix:**

| Domain | AI Capability (2026) | Primary Application | Limitation |
|--------|---------------------|---------------------|------------|
| **Drug discovery** | Target identification, molecule generation, ADMET prediction | 10-100× acceleration in hit-to-lead | Binding prediction ≠ clinical efficacy |
| **Protein structure** | Atomic-level prediction (AlphaFold3) | 200M+ structures predicted | Dynamic conformations still challenging |
| **Clinical diagnosis** | Pattern recognition in imaging, pathology | 700+ FDA-approved devices | Brittle to distribution shift |
| **Genomics** | Variant calling, gene-disease association | 10× faster genome interpretation | Rare variant interpretation remains difficult |
| **Materials science** | Property prediction, inverse design | 10-100× discovery acceleration | Synthesis feasibility often overestimated |
| **Literature analysis** | Cross-domain synthesis, hypothesis generation | 10,000 papers/night analysis | Hallucinated references; shallow understanding |
| **Clinical documentation** | Ambient scribing, note generation | 60% reduction in documentation time | Privacy and accuracy concerns in complex cases |

**Benchmark trajectory for scientific reasoning:**

| Benchmark | What It Measures | 2023 | 2024 | 2025 | 2026 | PhD Expert |
|-----------|-----------------|------|------|------|------|------------|
| **GPQA** | PhD-level reasoning | ~35% | ~50% | ~70% | ~90% | 65-80% |
| **USMLE** | Medical licensing | ~60% | ~87% | ~92% | ~96% | ~80-90% |
| **MoleculeNet** | Drug property prediction | ~75% | ~82% | ~88% | ~92% | ~85% |
| **BioProt** | Biological protocol comprehension | N/A | ~40% | ~60% | ~75% | ~80% |

## 14.2 The Drug Discovery Pipeline: AI Integration Stages

AI transforms drug discovery at every stage, but the degree of integration varies significantly.

**Pipeline stage analysis:**

| Stage | Traditional Time | AI-Assisted Time | AI Capability | Validation Requirement |
|-------|-----------------|------------------|---------------|----------------------|
| **Target identification** | 1-3 years | 2-6 months | AlphaFold, genetics AI: 8/10 | Wet-lab validation essential |
| **Hit discovery** | 1-2 years | 1-6 months | Generative chemistry: 7/10 | Biochemical assay required |
| **Lead optimization** | 2-4 years | 6-18 months | ADMET prediction: 6/10 | Animal model testing required |
| **Preclinical** | 1-2 years | 1-2 years | Toxicity prediction: 5/10 | Regulatory mandated; AI accelerates but cannot replace |
| **Phase I-III** | 6-10 years | 6-10 years | Trial design and monitoring: 4/10 | Fully regulated; AI assists in design |

**Economics of AI vs. traditional drug development:**

| Metric | Traditional | AI-Driven | Improvement |
|--------|------------|-----------|-------------|
| Cost per approved drug | $2-3B | $300-500M | 6-10× reduction |
| Phase I→approval success rate | 10% | 30-50% (projected) | 3-5× improvement |
| Time from target to Phase I | 5-7 years | 2-3 years | 50-60% reduction |
| VC investment (2025) | — | $14B (AI drug discovery) | 3.8× since 2023 |

**Landmark evidence:** INS018_055 (Insilico Medicine, 2024) — target to Phase II in under 3 years vs. 8-12 year traditional timeline. Recursion Pharmaceuticals had two AI-discovered cancer drugs in Phase II by 2025. Isomorphic Labs licensed candidates to Eli Lilly and Novartis for $1.2B pre-trial.

## 14.3 Clinical AI Deployment Matrix

Medical AI deployment varies dramatically by specialty, modality, and regulatory pathway.

**Clinical specialty application matrix:**

| Specialty | AI Maturity | FDA Approvals (2026) | Key Metric | Human Baseline | AI Performance |
|-----------|-------------|---------------------|------------|----------------|----------------|
| **Radiology** | Mature | 400+ | Lung cancer detection sensitivity | 88.4% | 94.4% |
| **Pathology** | Growing | 80+ | Prostate cancer false negative reduction | Baseline | 70% reduction |
| **Dermatology** | Growing | 50+ | Skin lesion classification accuracy | ~85% | ~90% |
| **Cardiology** | Emerging | 60+ | ECG interpretation accuracy | ~80% | ~85% |
| **Ophthalmology** | Mature | 30+ | Diabetic retinopathy detection | ~85% | ~94% |
| **Emergency medicine** | Experimental | 20+ | Sepsis prediction (12h early) | ~40% sensitivity | 80% sensitivity (Compass) |

**Deployment paradigm comparison:**

| Paradigm | Description | Accountability | Failure Mode |
|----------|-------------|---------------|--------------|
| **Second reader** | Human decides; AI reviews | Human retains accountability | Alert fatigue; automation bias |
| **First reader** | AI screens; human confirms | Shared liability | AI misses rare presentations |
| **Triage assistant** | AI prioritizes; human decides | Human accountable | Over-triaging; resource misallocation |
| **Co-pilot** | AI + human collaborative | Institutional policy | Role confusion; skill erosion |
| **Autonomous** | AI decides (narrow scope only) | Vendor + institution | Brittle to edge cases; no waiver |

## 14.4 AI-Augmented Clinical Workflow

**Documentation burden and AI resolution:**

| Activity | Physician Time (pre-AI) | Physician Time (with AI) | Improvement |
|----------|------------------------|------------------------|-------------|
| EHR documentation | 49% of workday | 20% of workday | 60% reduction |
| Direct patient care | 27% of workday | 42% of workday | 15pp increase |
| Chart review | 8% of workday | 4% of workday | 50% reduction |
| Order entry | 6% of workday | 3% of workday | 50% reduction |

**Clinical decision support impact (Mayo Clinic 2025 study):**

| Metric | Physician Alone | Physician + AI | Improvement |
|--------|----------------|----------------|-------------|
| Diagnostic accuracy | Baseline | +23% | 23% relative improvement |
| Time to diagnosis | Baseline | 40% faster | 40% reduction |
| Missed diagnosis rate | Baseline | -35% | 35% reduction |
| Test ordering appropriateness | Baseline | +18% | 18% improvement |

## 14.5 The Scientific Research Augmentation Framework

AI transforms the scientific method itself — augmenting each phase with capabilities that compound over time.

**Research phase augmentation:**

| Phase | Traditional | AI-Augmented | Bottleneck After AI |
|-------|-------------|--------------|---------------------|
| **Literature review** | Weeks; incomplete | Hours; 2× more relevant papers found | Synthesis quality assessment |
| **Hypothesis generation** | Domain-dependent intuition | Cross-domain pattern discovery | Experimental feasibility |
| **Experiment design** | Manual iteration | AI-optimized parameter space search | Lab capacity |
| **Execution** | Human-conducted; limited hours | Robotic lab 24/7 (10-100× acceleration) | Cost of automation infrastructure |
| **Data analysis** | Statistical testing | Deep pattern mining; anomaly detection | Interpretability |
| **Theory formation** | Human synthesis | AI-generated candidate theories | Validation: prediction-to-test ratio is 10:1 |
| **Peer review** | Weeks per paper; scale-limited | AI-assisted consistency checking (30% faster) | Detecting AI-generated fraud |

**Automated lab capability assessment:**

| Capability | 2023 | 2024 | 2025 | 2026 | Target |
|------------|------|------|------|------|--------|
| Self-driving lab throughput | 2× human | 5× human | 20× human | 50× human | 100× |
| Hypothesis-test cycles/day | 10 | 50 | 200 | 500 | 1,000+ |
| Cross-domain synthesis | Manual | AI-assisted | Semi-automated | Automated | Autonomous |

## 14.6 Research Integrity Threat Taxonomy

AI simultaneously solves and creates research integrity challenges.

| Threat Class | Mechanism | Scale (2026) | Detection Method | Mitigation |
|-------------|-----------|--------------|------------------|------------|
| **Paper mills** | AI generates plausible fake research | 15-30% of submissions at some journals | Tortured phrase detection; AI checking | Mandatory C2PA for submissions |
| **Data fabrication** | AI generates realistic experimental data | Growing | Statistical anomaly detection | Raw data archiving requirement |
| **Citation fraud** | AI hallucinates references | Common in LLM-generated papers | Reference verification | Mandatory human citation check |
| **Image manipulation** | AI alters scientific images | Significant | Forensic analysis AI | Pre-submission AI screening |
| **Peer review bypass** | AI generates fake reviewer identities | Emerging | Identity verification | Video verification protocols |

## 14.7 Regulatory Maturity and the Approval Lag

| Dimension | Current State (2026) | Gap | Target |
|-----------|---------------------|-----|--------|
| FDA AI device approvals | 882 total (2018-2026) | 1,200 pending applications | Streamlined review pathway |
| Algorithm change framework | Re-approval required for any change | AI cannot improve post-deployment | Continuous learning pathway |
| International harmonization | Fragmented (FDA/EMA/PMDA/NMPA) | Separate requirements ×4 | IMDRF unified framework (target 2028) |
| Liability framework | Pre-AI law | AI-assisted diagnosis liability unclear | AI medical liability doctrine needed |
| Continuous learning approval | 15 systems approved | Most AI frozen at approval | "Change protocol" approval not algorithm re-approval |

## 14.8 The Global Health Accessibility Impact

**The access-to-care gap AI can address:**

| Metric | High-Income Country | Low-Income Country | AI Solution |
|--------|--------------------|--------------------|-------------|
| Radiologists per 100K | 90 | 0.3 (Sub-Saharan Africa) | AI image triage on smartphone |
| Primary care access | Universal | 40% coverage (rural) | AI SMS triage (e.g., Babylon in Rwanda) |
| Diagnostic equipment | Full suite | Limited | AI analysis of phone-based diagnostics |
| Ophthalmology screening | Routine | Near zero | Phone-based retinopathy detection (96% accuracy) |

**The treatment gap:** AI can diagnose but cannot treat. The diagnostic capability exceeds therapeutic reach by a widening margin. The limiting factor in global health is no longer detection — it is intervention capacity.

## 14.9 The Human-AI Collaborative Model: Empirical Results

The central finding across every clinical and scientific domain: **human + AI outperforms either alone, but the collaborative interface determines the margin.**

| Collaboration Mode | Accuracy | Satisfaction | Liability | Skill Retention |
|-------------------|----------|--------------|-----------|-----------------|
| Human alone | Baseline | Highest | Clear | Full retention |
| Human + AI (optimal) | +15-25% | Moderate | Shared | Enhanced |
| AI alone (narrow task) | +5-15% | Lowest (patient) | Unclear | Erosion risk |
| AI alone (complex task) | -30% to +5% | Lowest | Vendor | N/A |

**The brittleness lesson (2024 brain hemorrhage case):** A major hospital's AI failed to detect a subdural hematoma because the CT was from a different manufacturer's machine than the training data. The oversight was caught by a human radiologist the next day. Distribution shift is the single largest unaddressed risk in clinical AI deployment.

## 14.10 Frontier Assessment: Three Revolutions

| Revolution | Readiness | Key Indicator | Target Year | Enabling Condition |
|------------|-----------|---------------|-------------|-------------------|
| 100× biology | 3/5 | First AI drug to market | 2030 | Validation pipeline capacity increase |
| Personalized medicine | 2/5 | Digital twin pilot completion | 2028-2030 | Regulatory pathway for continuous learning |
| Autonomous scientific discovery | 1/5 | First autonomous hypothesis → validation (closed loop) | 2030-2035 | Self-driving lab cost reduction |

**The economic dimension:** AI could reduce US healthcare spending by $200-400B/year (8-12%) through administrative automation, diagnostic efficiency, and personalized treatment. However, these savings are not equally distributed — the highest-income hospitals deploy first, and the global south is last in line for every advance.

**The verdict:** AI will not replace doctors or scientists. It will redefine what it means to be one — eliminating documentation and repetitive screening, and amplifying diagnosis, treatment planning, and patient relationships. The best clinicians of 2026 are not competing with AI. They are collaborating with it.
