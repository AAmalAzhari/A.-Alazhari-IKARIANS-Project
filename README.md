# A.-Alazhari-IKARIANS-Project
A project focusing on health data architecturing and integrating multimodal wearable APIs with subjective patient health data to power AI-driven longevity insights.


# Project Overview

## 1. Background and Context
This project establishes an Al-ready health data architecture for the lkarians platform, transitioning it from raw, multi-source wearable data ingestion into a structured framework optimised for Large Language Models (LLMs). By developing a 3-tier Extract, Transform, Load (ETL) pipeline, integrating Patient-Reported Outcomes Measurement Information System (PROMIS) T-scoring to close psychosocial data gaps, and designing external AI tools. The system achieves semantic interoperability, isolates true clinical signals from hardware noise and enforces clinical boundaries, ensuring the Ikarus Al agent delivers precise, hallucination-free, and actionable longevity insights.

## 2. Project Aim
To construct a comprehensive Al Readiness Framework that transforms complex, multi-source health data into structured, actionable insights. This involves achieving semantic interoperability, bridging psychosocial gaps, filtering noise, and implementing strict clinical guardrails.

## 3. Methods Used
(Details in `Data_Architecture/` and `Data_Assessment_and_Recommendations/`)

3.1. **Creating Data Dictionary and Diagrams:** 
Mapped and catalogued wearable API data across four major brands (Apple, Garmin, Google, Samsung) and created a comprehensive Data Dictionary to map varying brand-specific metrics into unified "Ikarians Standard Variables" to achieve semantic interoperability. Also created Data Flow Diagram and Health Data Ecosystem Map (refer to `Diagrams/`) to illustrate how data flows within the system.

3.2. **Objective Data Normalisation:** 
Built a 3-Tier ETL pipeline in R to translate the brand-specific metrics into the unified "Ikarians Standard Variables" and apply 24-hour time- window aggregations to protect the LLM's token limits.

3.3. **Subjective Data Integration:** 
Used PROMIS short forms, MEDAS and AUDIT-C to convert qualitative human experiences into objective, standardised scores.

3.4. **Signal vs. Noise Modeling:** 
Used intra-individual Z-scoring and cross-referencing of subjective/objective signals to filter true signals. 



## 4. Main Results and Outputs
(Details in `Implementation_and_Data_Management/` and `AI_Readiness_and_Insight_Discovery/`)

4.1. **Data Standardisation and Compound Signals:**
The ETL pipeline successfully outputs unified daily summaries, granting the Al a clear, chronologically aligned timeline. By normalising both objective wearable data and subjective PROMIS T-scores, the system was able to construct high-value compound signals.

4.2. **Subjective Data Integration:**
Successfully transformed qualitative data into objective scores by integrating PROMIS (Patient-Reported Outcomes Measurement Information System) Short Forms.

4.3. **External Al Tools Integration:** 
Developed AI tools to improve insights generated and efficiency. Suggested tools included:
1. Signal vs. Noise Validator.
2. Biometric-Pharmacological Cross-Referencer.
3. Nutrition Facts Label & Portion Scanner.

## 5. Implications for Ikarians
This framework transforms Ikarians into a clinically safe, hardware-agnostic medical companion. By solving semantic interoperability and translating subjective data into objective mathematics, it provides a true 360-degree patient view. Additionally, integrating external tools to query medical databases, estimate dietary intake and validate signals, ensures the Ikarus Al agent can draw relevant insights more accurately and efficiently.
