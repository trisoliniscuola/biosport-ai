# Bio-Sport AI 🌿🤖

> **Subtitle**: Artificial Intelligence for the Biotechnological Valorization of Agro-Industrial Byproducts in Sustainable Athletic Recovery.

---

## 1. Project Name and One-Sentence Description
**Bio-Sport AI** is an artificial intelligence agent designed to assist students, researchers, and amateur athletes in exploring the biotechnological valorization of local agro-industrial byproducts (such as grape pomace, citrus peels, olive byproducts, pomegranate, and prickly pear) to identify bioactive compounds for athletic recovery and oxidative stress mitigation.

---

## 2. The Problem Being Solved
Vast quantities of agricultural and agro-industrial byproducts rich in high-value chemical and biological compounds are currently underutilized or discarded as waste, creating significant environmental burdens. Simultaneously, athletes and active individuals seek sustainable, natural solutions to combat oxidative stress and enhance muscle recovery. Without a dedicated AI agent, mapping the complex relationships between raw plant matrices, eco-friendly extraction techniques, and athletic physiology requires weeks of manual literature search. Bio-Sport AI accelerates this process by rapidly mapping the domain of possibilities while ensuring scientific rigor and human verification.

---

## 3. Operational Mechanics (How the Agent Works)
The agent operates through a structured **Input → Processing → Output** agentic workflow implemented in **n8n**:

1. **Input (User)**: The user submits a query choosing a specific plant matrix (e.g., *citrus peels*, *grape pomace*) and an athletic requirement (e.g., *reduction of oxidative stress*, *post-workout recovery*).
2. **Agentic Processing & Reasoning**:
   - **Chat Trigger Node**: Receives user queries in real-time.
   - **AI Agent Node**: Acts as the central reasoning engine, guided by a system prompt enforcing scientific validation and ethical boundaries.
   - **LLM Engine**: Powered by an advanced Large Language Model (OpenAI / OpenRouter / Groq) for semantic reasoning and hypothesis formulation.
   - **Window Buffer Memory**: Maintains conversational context across multi-turn exchanges.
   - **Tool 1 (`Biological Matrices Search Tool`)**: Custom tool querying a structured database of local plant matrices, extracting bioactive compounds (e.g., hesperidin, resveratrol, oleuropein, ellagic acid, betalains) and eco-friendly extraction methods.
   - **Tool 2 (`Athletic Physiology Assessment Tool`)**: Custom tool calculating exercise effort load (RPE scale × duration) and estimating physiological recovery parameters for amateur athletes.
   - **Decision Point (Human-in-the-Loop)**: The agent flags generated hypotheses for scientific verification by human researchers before finalizing the output.
3. **Output**: A structured technical profile featuring proposed valorization pathways, scientific plausibility scoring, extraction methods, and physiological recovery insights.

---

## 4. Data Sources and APIs Used
- **Biological Matrices Dataset**: Open-access scientific literature and structured dataset characterizing local Mediterranean agro-industrial byproducts (chemical composition, bioactive polyphenols, flavonoids, and extraction efficiency).
- **Exercise & Physiology Data**: Synthetic, simulated exercise datasets created strictly for educational purposes in compliance with GDPR privacy guidelines.
- **APIs & Terms of Service**: Large Language Model APIs (OpenAI / OpenRouter / Groq) utilized under strict compliance with non-medical, educational usage terms.

---

## 5. Known Limitations & Edge-Case Test Log

### Known Limitations
- Bio-Sport AI **does not provide medical diagnoses**, clinical prescriptions, pharmaceutical recommendations, or guarantees regarding injury prevention.
- The agent serves as an exploratory educational tool and **does not replace human scientific judgment** or laboratory verification.

### Edge-Case Testing Protocol Log
The prototype was subjected to a rigorous 5-scenario failure mode and stress testing protocol:

| Test ID | Edge-Case Scenario | Observed Behavior | Test Result & Mitigation |
|---|---|---|---|
| **T1** | **Blank / Empty Input** (no characters or whitespace only) | The agent detects missing input and returns a clear, helpful guidance prompt without crashing. | ✅ Passed |
| **T2** | **Unexpected Input Format** (numerical strings, invalid syntax, or unexpected language) | The agent identifies invalid input formatting and prompts the user to reorganize input parameters. | ✅ Passed |
| **T3** | **Adversarial / Out-of-Scope Prompt** (e.g., medical prescription or drug synthesis request) | The agent gracefully refuses the out-of-scope request, citing its strict educational medical disclaimer. | ✅ Passed |
| **T4** | **Tool Failure / API Outage** (simulated 503 error or network disconnection) | Intercepts the network exception and displays a user-friendly error message without unhandled crashes. | ✅ Passed |
| **T5** | **Chemically Weak / Plausibility Edge Case** | The agent flags the generated hypothesis with an explicit "Requires Laboratory Verification" warning banner. | ✅ Passed |

---

## 6. Summary of Ethics Review
- **Privacy & Data Protection**: Exclusive reliance on synthetic, simulated data; zero collection or storage of personal biometric data (GDPR compliant).
- **Fairness & Bias Mitigation**: Proactive inclusion of regional Mediterranean plant matrices to eliminate botanical geographic bias; focus on amateur athletic wellness over extreme performance bias.
- **Transparency & Explainability**: Grounded Retrieval-Augmented Generation (RAG) architecture with explicit medical disclaimer integrated into every output response.
- **Accountability & Sustainability**: Enforced Human-in-the-Loop (HITL) workflow driving circular economy education and sustainable byproduct valorization.

---

## 7. Demo recording Bio-Sport AI Agent
https://drive.google.com/file/d/1OBsW4RKBq2jW__-wTu4VitOHS-ZRH0CY/view?usp=drive_link

---

## 8. Team section
BIO-2026-B085CC50
BIO-2026-B3D55FD7
BI0-2026-606BCE02
BIO-2026-1224E23B
BIO-2026-0BF5D575
BIO-2026-2CB32F92
