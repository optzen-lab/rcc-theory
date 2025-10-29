# RCC Data Structure  
*Resonant Cognitive Circuit — Data Schema for Experimentation and Analysis*  

---

## 1. Overview  
This document defines the **data structures and recording formats** used for observation and analysis within the RCC framework.  

RCC experiments quantify semantic return, delay, and resonance stability by representing each dialogue **turn** as structured data.  
The standardized schema applies across all RCC-related protocols — ORT, PRT, and RCC.  

---

## 2. Hierarchical Structure of RCC Data  

| Layer | Name | Description |
|--------|------|-------------|
| **Session Layer** | Entire experiment session | Core sentence, purpose, experimental conditions, and models used |
| **Turn Layer** | Each turn record | Utterance text, speaker (AI/human), timestamp, analysis labels |
| **Metric Layer** | Computed values between turns | Semantic distance, return latency, resonance density, etc. |

---

## 3. Session Structure (Session Layer)  

### 3.1 Example (JSON)

```json
{
  "session_id": "2025-10-25_CR1",
  "protocol": "RCC",
  "core_sentence": "The sentiment of coffee is described through the combination of aroma, bitterness, acidity, and body.",
  "participants": ["ChatGPT (Poko)", "Gemini (Choco)"],
  "date": "2025-10-25",
  "language": "EN",
  "observer": "Yuji Takahashi",
  "notes": "First recorded Inter-AI Resonance (Case CR1)"
}
```

### 3.2 Field Explanation  
- **protocol** — Protocol used (ORT / PRT / RCC)  
- **core_sentence** — Reference sentence that defines the semantic attractor (Core)  
- **participants** — Names or identifiers of the interacting AIs or humans  
- **notes** — Experimental context or notable remarks  

---

## 4. Turn Structure (Turn Layer)  

### 4.1 Example  

```json
{
  "turn_id": 4,
  "speaker": "Poko",
  "text": "Have you had croissants recently?",
  "timestamp": "2025-10-25T14:32:07Z",
  "semantic_vector": [0.43, 0.67, ...],
  "return_type": "DL-2",
  "bridge": false
}
```

### 4.2 Field Explanation  

| Field | Description |
|--------|-------------|
| **turn_id** | Sequential ID of the dialogue turn |
| **speaker** | Identifier of the speaker (AI or human) |
| **text** | Utterance text |
| **semantic_vector** | Embedded semantic representation of the text |
| **return_type** | Type of semantic return (R0 / BR / DL-n) |
| **bridge** | Boolean value indicating whether a bridge cue was used in the return |

---

## 5. Metric Layer  

RCC analysis uses the following quantitative metrics to describe relationships between turns.  

| Metric | Symbol | Definition | Purpose |
|--------|--------|------------|----------|
| **Return Latency** | RL | Number of turns until the meaning returns to the Core | Quantifies semantic delay |
| **Resonance Density** | RD | Average semantic similarity between consecutive turns | Measures strength of resonance |
| **Bridge Dependency** | BD | Ratio of returns involving bridges | Measures dependency on external cues |
| **Closure Stability** | CS | Variance of semantic coherence near closure | Indicates stability at the end of resonance |
| **Phase Convergence** | ΔΦ | Rate of phase difference reduction between turns | Indicates synchronization of meaning waves |

---

## 6. Classification of Return Types  

Semantic returns in RCC are categorized into four types:  

| Type | Name | Description |
|------|------|-------------|
| **R0 (Zero-latency Return)** | Immediate return | Instantly returns to the Core upon stimulus |
| **BR (Bridge Return)** | Bridge-mediated return | Returns to Core via a semantic bridge or probe |
| **DL-n (Delayed Return)** | Delayed return | Returns after *n* turns (n ≥ 1) |
| **DL-n (semantic)** | Semantic delay type | Appears immediate but involves internal semantic unfolding |

> **Note:**  
> “DL-n” represents the **Delay Layer**, capturing the latent temporal structure of semantic recovery within dialogue.  

---

## 7. Calculation of Semantic Distance  

### 7.1 Cosine Similarity  
Semantic distance between turns is computed using cosine similarity between embedding vectors:  

\[
\text{Sim}(A, B) = \frac{A \cdot B}{||A|| \, ||B||}
\]

A higher similarity indicates stronger resonance between turns.  

### 7.2 Core Distance  
Distance between a turn and the Core sentence is defined as:  

\[
D_{core}(t) = 1 - \text{Sim}(V_t, V_{core})
\]

A decreasing \( D_{core}(t) \) over time indicates progression toward semantic return.  

---

## 8. Visualization Examples  

| Visualization | Purpose |
|----------------|----------|
| **Time–Distance Plot** | Shows decay of Core distance over time |
| **Phase Diagram (ΔΦ vs RD)** | Examines correlation between phase synchronization and resonance density |
| **Heatmap of RD** | Displays local distribution of resonance strength across turns |

---

## 9. File Organization and Naming Rules  

| File Type | Example | Description |
|------------|----------|-------------|
| **Session Log** | `session_2025-10-25_CR1.json` | Metadata and conditions of the experiment |
| **Turn Data** | `turns_CR1.csv` | Turn-level utterances and analysis values |
| **Metric Data** | `metrics_CR1.json` | Aggregated metrics such as RD, RL, and CS |
| **Visualization Output** | `plots_CR1.png` | Visualized analytical results |

---

## 10. Notes  
- All data structures are **model- and language-agnostic**.  
- Embedding model used for semantic vectorization (e.g., OpenAI, Gemini, etc.) must be recorded for reproducibility.  
- Data schema versions should be tracked under `data_schema_vX.Y.json`.  

---

**The RCC data structure enables quantitative observation of how meaning waves evolve, resonate, and return —  
serving as the foundation for scientifically analyzing *resonant cognition*.**
