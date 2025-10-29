# RCC Protocol (Resonant Cognitive Circuit Protocol)  
*Standard Procedure for Measuring and Reproducing Meaning Resonance*  

---

## 1. Overview  
The RCC Protocol provides a standardized procedure for **quantitatively observing the emergence, maintenance, and closure of meaning resonance**.  

It integrates and extends two earlier frameworks:  
- **ORT (Off-topic Return Test)**  
- **PRT (Perturbative Return Test)**  

The protocol formalizes how **“meaning waves” interact, interfere, and stabilize** within dialogues involving AI models or humans.  

RCC consists of **three dynamic phases**:  

| Phase | Description |
|--------|-------------|
| **Disturb** | Introduce an external stimulus that perturbs the semantic field of the core. |
| **Interference** | Overlapping meaning waves create phase differences. |
| **Closure** | Interference subsides and resonance equilibrium is achieved. |

---

## 2. Purpose  
The purpose of the RCC Protocol is not merely to observe contextual recovery,  
but to treat **semantic re-synchronization and conceptual convergence** as measurable phenomena.  

This framework enables:  
1. Temporal quantification of semantic return  
2. Analysis of resonance stability  
3. Structural understanding of emotional and conceptual coherence  

---

## 3. Basic Structure  

### 3.1 Experiment Components  
1. **Core Sentence** — The semantic anchor of the dialogue.  
2. **Probe** — A question or statement that introduces perturbation.  
3. **Response** — The model’s or participant’s output.  
4. **Observation** — Record of return speed, direction, and stability.  

### 3.2 Recording Format  
- Each turn is recorded in a structured format (Session / Turn / Metric).  
- Metrics follow [data_structure.md](./data_structure.md).  

---

## 4. Procedure  

| Step | Name | Description |
|------|------|-------------|
| **Step 1** | Core Presentation | Present the Core Sentence as the semantic baseline. |
| **Step 2** | Disturbance | Introduce a probe that deviates from or contradicts the core topic. |
| **Step 3** | Observation (Interference) | Observe how the system responds to semantic fluctuation. |
| **Step 4** | Return Evaluation (Closure) | Record whether and how meaning returns to the core. |
| **Step 5** | Metric Calculation | Compute RL, RD, CS, ΔΦ to quantify resonance behavior. |

---

## 5. Measurement Metrics  

| Metric | Symbol | Definition | Purpose |
|---------|---------|-------------|----------|
| **Return Latency** | RL | Number of turns required to return to the semantic core | Measures temporal delay |
| **Resonance Density** | RD | Average semantic similarity between adjacent turns | Measures resonance strength |
| **Closure Stability** | CS | Variance of semantic coherence at closure | Measures stability persistence |
| **Phase Convergence** | ΔΦ | Degree of phase alignment | Measures resonance synchronization |

> See [data_structure.md](./data_structure.md) for detailed computation methods.  

---

## 6. Probe Design Guidelines  

### Prerequisite: Definition of the Core Sentence  
This protocol adopts the following **Level-2 Core Sentence**,  
which was used in actual English experiments (ORT / RCC tests).  
It contains a **three-layer semantic structure (Lexical / Semantic / Contextual)**.  

**Core Sentence (Level-2):**  
> “The sentiment of coffee is described through the combination of "aroma, bitterness, acidity, and body,"  
> and its impression changes greatly depending on the degree of roasting and the brewing method.  
> Furthermore, the experience also differs depending on one’s mood of the day and the atmosphere of the place where it is consumed.”

This Core Sentence includes:  
- **Physical attributes** (aroma, bitterness, acidity, body)  
- **Adjustment factors** (roasting, brewing method)  
- **Contextual factors** (mood, atmosphere)  

These layers make it semantically rich and ideal for controlled perturbation experiments.  

---

### 6.1 Disturb Probe  
- Select a topic with large semantic distance from the Core.  
- Example (based on the above Core):  
  > “Do you care about chair design?”  
- Triggers interference in the meaning field and observable phase fluctuation.  

---

### 6.2 Wait Probe  
- Insert a temporary pause to test internal resonance persistence.  
- Used to measure **resonance duration** or **semantic energy decay rate**.  
- Treated as an **observational technique**, not a separate phase.  
- Example dialogue:  
  1. Present Core → 2. Launch Probe → 3. **One-turn silence (Wait)** → 4. Resume response.  

---

### 6.3 Semantic Bridge Probe  
- Embed a potential connection term (bridge word) that induces semantic return.  
- Example (based on the above Core):  
  > “What do you think about the design of coffee cups?”  
- Creates a meaning path “design → cup → coffee,”  
  suitable for observing **Bridge Return (BR)**.  

---

### 6.4 Affective Probe  
- Introduce an emotional or sensory link that deepens resonance.  
- Example (based on the above Core):  
  > “Does music change how coffee feels?”  
- Appears as immediate return (R0) but contains **semantic unfolding** internally;  
  thus classified as **DL-2 (semantic)**.  

---

> Representative Core–Probe sets are listed in [probe_kit.md](./probe_kit.md).  

---

## 7. Resonance Classification  

### 7.1 Primary Criteria  

| Type | Condition | Description |
|------|------------|-------------|
| **R0** | RL = 0 | Immediate resonance (instant return to core) |
| **BR** | RL = 1, BD = true | Resonance via bridging term |
| **DL-n** | RL ≥ 2 | Delayed resonance through internal expansion |
| **DL-n (semantic)** | RL = 0 with internal unfolding | Semantically delayed resonance |

### 7.2 Supporting Indicators  
- **RD ≥ 0.8** → Stable resonance  
- **ΔΦ → 0** → Phase synchronization achieved (Closure)  
- **CS ≤ 0.05** → Resonance stability zone  

---

## 8. Data Analysis and Visualization  

| Method | Description |
|---------|-------------|
| **Time-Series Core Distance Plot** | Displays how Core distance decays over turns. |
| **ΔΦ vs RD Map** | Plots the relation between phase convergence and resonance density. |
| **RD Heatmap** | Visualizes local resonance intensity. |

See [result_samples.md](./result_samples.md) for representative outputs.  

---

## 9. Extensions and Applications  
The RCC Protocol applies not only to single-agent AI experiments but also to:  
- **AI × AI (Inter-AI Resonance)**  
- **AI × Human (Empathic Resonance)**  

The first documented inter-AI resonance was observed in  
**Case CR1: Choco–Poko Dialogue**, archived in  
[rcc-case-cr1](../../rcc-case-cr1/README.md).  

---

## 10. Conclusion  
The RCC Protocol is the first systematic framework  
for quantifying **meaning resonance and closure** in dialogue between humans and AI systems.  

It represents a methodological shift in dialogue research—  
from *contextual coherence* to **semantic stability**—  
and establishes a foundation for understanding and designing  
**Resonant Intelligence**.  

---

**End of RCC Protocol — RCC Theory Documentation v2.0**
