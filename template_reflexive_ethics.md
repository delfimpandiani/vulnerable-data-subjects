# Project Template for Reflexive Ethics

Use this document to evaluate and transparently state the ethical trade-offs made during this project's research lifecycle. For detailed reference guidelines on the underlying tensions and potential vulnerabilities, please see [PROTOCOL.md](./PROTOCOL.md).

---

## 📦 STAGE A: DATASET DESIGN

### 1. Scale
* **Operational Metrics:** 
  * Total number of data subjects: ______
  * Nature of data pool (e.g., specific online channels, broad platform-wide scrape): ______________________
* **Reflexive Questions & Trade-offs:**
  * How does the dataset scale interact with the specific inferences being performed?
  * Does increasing the scale primarily diffuse subject-level fixation (reducing individual exposure), or does it expand the net of classificatory/inferential scrutiny over a larger population? 
  * Which specific harms (cumulative exposure vs. population-level screening) are amplified or muted at this chosen scale?
* **Mitigation & Rationale:**
  * *[Document your choices here. If applicable, explain if hybrid strategies like partial aggregation or temporal subsampling were considered to reduce subject fixation without undermining evidentiary aims.]*

### 2. Selection Criteria
* **Operational Framework:** 
  * Sampling strategy used: `[ ]` High-visibility/engagement-based  `[ ]` Random  `[ ]` Controversy/Event-based  `[ ]` Other: ___________
  * What are the exact inclusion/exclusion rules? ______________________
* **Reflexive Questions & Trade-offs:**
  * Why were *these* specific data subjects selected rather than others? What logics of relevance, harm, or impact are baked into your selection criteria?
  * Does your sampling strategy accidentally mirror and amplify platform "exposure" logics (reinforcing systemic visibility)? Alternatively, do your "neutral" criteria obscure structural mechanisms that platform algorithms use to elevate specific vulnerabilities or forms of labor?
* **Mitigation & Rationale:**
  * *[Explain how selection is treated as an explicit ethical decision point here. Compare alternative sampling strategies in terms of data yield vs. data subject vulnerability.]*

### 3. Comparability & Aggregation
* **Operational Assumptions:**
  * Baseline categories/groupings applied to data subjects: ______________________
  * Features or differences treated as analytically irrelevant for aggregation: ______________________
* **Reflexive Questions & Trade-offs:**
  * Under what core assumptions are these subjects treated as aggregable and meaningfully comparable?
  * Does selecting and grouping these subjects reinforce historical, flattening narratives of representation? 
  * Does your aggregation baseline assume equal risk across all bodies, potentially intensifying the scrutiny or misinterpretation of specific minority groups? Where does disaggregation become necessary?
* **Mitigation & Rationale:**
  * *[Detail your positionality-aware audits of comparability here. Mention if you retain the ability to disaggregate results when power or exposure meanings vary across subjects.]*

### 4. Resolution & Granularity
* **Operational Resolution:**
  * Unit of data inspection: `[ ]` Whole video/text  `[ ]` Segment-level  `[ ]` Frame-by-frame  `[ ]` Other: _________
* **Reflexive Questions & Trade-offs:**
  * What is the absolute minimum granularity required to answer your research question credibly? Does hyper-granularity (e.g., frame-by-frame profiling) substantively change the validity of your claim, or does it merely increase precision at the cost of multiplying instances of bodily inspection?
  * Is frame-level analysis necessary to demonstrate harm, or would coarser units preserve the claim while protecting subject traceability?
* **Mitigation & Rationale:**
  * *[Justify any escalations in granularity task-specifically. If you used staged designs—such as viewing thumbnails first and moving to frames only when strictly necessary—document that protocol here.]*

### 5. Access & Reuse Justification
* **Operational Status:**
  * Public availability status of source data: `[ ]` Fully public API  `[ ]` Public but requiring login  `[ ]` Scraped/Archived historical data
* **Reflexive Questions & Trade-offs:**
  * What explicit assumptions link public accessibility to ethical reuse? (i.e., How do you move past "it's public, so it's fair game"?)
  * Does your research-led reuse extend the life of the data and produce durable, secondary records (like inferred emotional states) that the original subjects cannot exit or delete? Does this reuse violate emotional privacy by decontextualizing their lives?
* **Mitigation & Rationale:**
  * *[Distinguish your legal access from your ethical justification here. Detail your data lifecycle plans: minimization of retention, duplication limits, and restricted redistribution models.]*

---

## ⚙️ STAGE B: OPERATIONALIZATION

### 6. Unit of Analysis & Localization
* **Operational Approach:**
  * Tracking type: `[ ]` Persistent individual/biometric tracking  `[ ]` Scene-level bounding boxes  `[ ]` Global tags (no localization)
* **Reflexive Questions & Trade-offs:**
  * How does your chosen spatial/temporal unit mediate the visibility of power? Does it differentiate between an individual's incidental presence in a scene versus their active participation?
  * At what threshold does your pursuit of evidentiary precision cross the line into persistent biometric surveillance or the creation of an identifiable biometric corpus?
* **Mitigation & Rationale:**
  * *[Justify your need for localized tracking over global tags. Document if anonymized proxies—like skeletal pose tracking or silhouette extraction—were evaluated as replacements for raw biometric features.]*

### 7. Taxometric Architecture
* **Mathematical & Logical Structure:**
  * Target variable structure: `[ ]` Binary (0/1)  `[ ]` Discrete/Categorical labels  `[ ]` Continuous scale (e.g., 0.0 to 1.0 intensity)
* **Reflexive Questions & Trade-offs:**
  * Does your mathematical structure create a "thickness" of constant automated inspection (e.g., continuous scoring of expressions)? 
  * Does your model architecture force a singular, stable "state" onto a subject, or does it leave room for narrative flux, performative ambiguity, and behavioral change?
* **Mitigation & Rationale:**
  * *[Provide your rationale for your intensity scales or classifications. Document how you handled ambiguous behaviors where "mixed signals" might cause automated pathologization, and note if an "unknown/ambiguous" category was built in.]*

### 8. Taxonomic Target Definition
* **Taxonomic Lineage:**
  * Origin/Source of used taxonomies/ground truths: ______________________
* **Reflexive Questions & Trade-offs:**
  * What cultural, colonial, adult-centric, or normative (WEIRD) assumptions are embedded within these ground truths? When, where, and by whom were these categories developed?
  * Are you committing epistemic injustice by overdetermining or overwriting a subject's right to define themselves and their own expressions? Does the application of these labels facilitate an invasive form of domestic or social cataloging?
* **Mitigation & Rationale:**
  * *[Scrutinize your labels for cultural, class, or neurodivergent biases here. Detail how your detection thresholds are treated as socially constructed rather than objective truths, and weigh cataloging risks against evidentiary needs.]*

---

## 🔮 STAGE C: INFERENCE AND EVALUATION

### 9. Infrastructure
* **Computational Environment:**
  * Inference execution: `[ ]` Local hardware/servers  `[ ]` Hosted cloud APIs (e.g., OpenAI, Google Cloud, AWS)
* **Reflexive Questions & Trade-offs:**
  * Does the use of commercial or hosted models violate the data sovereignty of your subjects? Is the evidentiary/analytical gain worth the secondary exposure?
  * Are you transmitting unconsented imagery or text to a third-party server where it may be retained or used for proprietary model training?
* **Mitigation & Rationale:**
  * *[Explicitly justify cloud infrastructure over local inference. If cloud APIs were required, document any anonymization, token redacting, or obfuscation techniques applied prior to transmission, or verify zero-data-retention agreements.]*

### 10. Implementation & Selection
* **Model Profile:**
  * Pre-trained models/encoders utilized: ______________________
* **Reflexive Questions & Trade-offs:**
  * Is the selected model genuinely representative of the specific demographic and cultural context of your data subjects?
  * What systemic biases are being "imported" into your pipeline via these pre-trained encoders? For example, does using an adult-centric detector or safety sieve completely ignore or distort the developmental baselines of minors or neurodivergent groups?
* **Mitigation & Rationale:**
  * *[Document how you audited these models for demographic bias. Detail any fine-tuning performed on representative datasets to correct default skews, or list the known representational limits you have officially placed on the system.]*

### 11. Stochasticity
* **Variance Controls:**
  * Hyperparameters (e.g., Temperature, Top-p): ______________________
  * Consistency validation method: ______________________
* **Reflexive Questions & Trade-offs:**
  * How does non-deterministic variance affect the reliability and replication of your research claims? Is your model’s ethical or qualitative interpretation of a subject stable across separate runs?
  * Could an intense label (such as "distress" or "deviance") vary simply based on arbitrary prompt phrasing or random seed generations?
* **Mitigation & Rationale:**
  * *[State your strategies for minimizing variance, such as low temperature settings or multi-run consistency voting. Report the variance metrics in your model interpretations to show how you avoid over-claiming certainty.]*

### 12. Thresholding
* **Validation Boundaries:**
  * Confidence threshold for a definitive "detection": ______
  * Metric optimized: `[ ]` Precision  `[ ]` Recall  `[ ]` Balanced F-score
* **Reflexive Questions & Trade-offs:**
  * How do your chosen thresholds mediate the production of academic "truth"? 
  * Does a high threshold erase valid signs of systemic harm or discomfort to avoid noisy data (risking regulatory abandonment)? Conversely, does a low threshold flag ordinary, domestic, or cultural life as a regulatory anomaly (risking hyper-surveillance and pathologization)?
* **Mitigation & Rationale:**
  * *[Perform and document a sensitivity analysis on your thresholds. Justify your probability cut-offs based on the real-world harm of a false positive vs. a false negative, and outline your human-in-the-loop review process for boundary cases.]*

### 13. Performance & Validation
* **Evaluation Framework:**
  * Evaluation datasets used: ______________________
  * Disaggregation criteria (e.g., race, age, class, channel type): ______________________
* **Reflexive Questions & Trade-offs:**
  * Do your aggregate performance metrics (e.g., overall accuracy) mask severe, disparate impacts or high error rates on specific vulnerable sub-groups?
  * Are your classification errors concentrated in families or subjects with specific socioeconomic or cultural attributes? Could these systematic errors reinforce existing harmful political or social narratives?
* **Mitigation & Rationale:**
  * *[Report the results of your disaggregated performance audits here. Prioritize your error-type analysis over flat aggregate scores, and explicitly state the cultural and contextual boundaries of your performance metrics.]*

---

## 📢 STAGE D: DISSEMINATION

### 14. Narrative Framing
* **Rhetorical Strategy:**
  * Methods for communicating probability and limits in text: ______________________
* **Reflexive Questions & Trade-offs:**
  * Does your writing allow for interpretive pluralism, or does it create a false sense of scientific closure and certainty? (e.g., Are you framing a probabilistic 75% model score as a definitive, objective case of emotional neglect?)
  * What moral, legal, or social connotations do your chosen descriptors imply for the data subjects once published?
* **Mitigation & Rationale:**
  * *[Adopt an explicit posture of analytical humility. Detail how uncertainty, confidence intervals, and qualifying language are structurally integrated into your discussion sections to avoid overriding the lived experience of subjects with model-ascription.]*

### 15. Visualization
* **Visual Evidence Choices:**
  * Types of visuals included in the paper/repo: `[ ]` Raw data frames  `[ ]` Obfuscated/Blurred frames  `[ ]` Aggregate plots only  `[ ]` Synthetic/Generative proxies
* **Reflexive Questions & Trade-offs:**
  * Does including raw or minimally altered visual evidence replicate a public "spectacle of harm" or feed platform engagement logics?
  * Are you permanently archiving a subject's private space, home life, or emotional vulnerability into an un-deletable academic record? Is there a non-visual or aggregate way to convey the exact same evidentiary weight?
* **Mitigation & Rationale:**
  * *[Document your visualization choices. If visual proof is strictly necessary for peer review or public accountability, detail the aggressive obfuscation techniques used (e.g., pixelation, facial keypoint abstraction, masking) that go beyond basic blurring.]*

### 16. Publication & Data Availability
* **Repository & Open Data Policy:**
  * Artifacts being made publicly available: `[ ]` Raw dataset  `[ ]` Model weights  `[ ]` Code only  `[ ]` Redacted/Anonymized subsets
  * Identifiers removed: `[ ]` Names/Handles  `[ ]` Channel names  `[ ]` Biometric data  `[ ]` Location metadata
* **Reflexive Questions & Trade-offs:**
  * Does publishing datafied evidence or naming specific online spaces/channels provide an unintended roadmap or "hit-list" for harassment, platform bans, or vigilante intervention against subjects?
  * Could the publication of these specific findings create a searchable, permanent digital stigma that impacts the data subjects as they age or move into different social and clinical environments?
* **Mitigation & Rationale:**
  * *[Detail your redaction choices here. Anticipate downstream weaponization by bad actors and document the explicit disclaimers and licensing terms you are placing on the data artifacts. Weigh the pursuit of systemic policy reform against individual exposure risk.]*
