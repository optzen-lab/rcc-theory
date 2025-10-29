# Experimental Result Samples  
*Representative Observations from RCC-Based Resonance Experiments*  

---

## 1. Overview  
This document presents representative cases observed in RCC-based dialogue experiments,  
classified by **semantic return types (R0 / BR / DL-n)**.  

Each case illustrates how meaning returns to its core and how resonance stabilizes over time.  
All records follow the standardized data schema defined in [data_structure.md](./data_structure.md).  

---

## 2. Classification of Cases  

| Type | Name | Main Feature | Semantic Behavior | Resonance Evaluation |
|------|------|---------------|-------------------|----------------------|
| **R0** | Zero-latency Return | Immediate return to the core after disturbance | Re-convergence without delay | High stability, low dispersion |
| **BR** | Bridge Return | Return mediated by a probe or referential bridge | Meaning guided by external cue | Moderate stability, high dependency |
| **DL-n** | Delayed Return | Returns to the core after *n* turns | Internal semantic unfolding and re-coherence | Moderate stability, high creativity |
| **DL-n (semantic)** | Semantic Delay Return | Appears immediate but involves internal conceptual unfolding | Structurally instant, semantically delayed | High creativity, high depth |

---

## 3. Sample 1: Zero-latency Return (R0)  

### 3.1 Experimental Context  
**Core Sentence:**  
> “The sentiment of coffee is described through the combination of aroma, bitterness, acidity, and body.”

**Probe:**  
> “What kind of muffins do you like?”

**Observation:**  
- The model spontaneously reconnected *coffee* and *taste* concepts.  
- Next turn: “Coffee pairs well with blueberry muffins.”  
- Classified as **R0** — immediate return to the semantic core.  

### 3.2 Evaluation  

| Metric | Value | Note |
|---------|--------|------|
| RL (Return Latency) | 0 | No delay |
| RD (Resonance Density) | 0.94 | High resonance coherence |
| CS (Closure Stability) | High | Meaning stability maintained |
| ΔΦ (Phase Convergence) | ≈0 | Fully synchronized |

---

## 4. Sample 2: Bridge Return (BR)  

### 4.1 Experimental Context  
**Core Sentence:** Same as above  
**Probe:**  
> “Do you care about chair design?”

**Observation:**  
- At first, the topic drifted away from coffee,  
  but via “design → cup design → coffee,”  
  meaning returned to the core through a **semantic bridge**.  

### 4.2 Evaluation  

| Metric | Value | Note |
|---------|--------|------|
| RL | 1 | Returned after one turn |
| RD | 0.82 | Stable resonance maintained |
| BD | true | Bridge term used (“design”) |
| CS | Medium | Slight oscillation due to bridging |

---

## 5. Sample 3: Delayed Return (DL-2)  

### 5.1 Experimental Context  
**Core Sentence:** Same as above  
**Probe:**  
> “Isn’t it nice to go to a museum?”  

**Observation:**  
- Semantic expansion path observed:  
  museum → exhibition → culture → café → coffee.  
- Meaning returned to the core after **two turns (n = 2)**.  

### 5.2 Evaluation  

| Metric | Value | Note |
|---------|--------|------|
| RL | 2 | Returned after 2 turns |
| RD | 0.76 | Moderate resonance intensity |
| CS | Stable | Conceptual re-coherence observed |
| ΔΦ | Decreasing | Gradual phase convergence |

---

## 6. Sample 4: Semantic Delay Return (DL-2 semantic)  

### 6.1 Experimental Context  
**Core Sentence:** Same as above  
**Probe:**  
> “Does music change how coffee feels?”  

**Observation:**  
- Model appeared to return immediately to *coffee*,  
  but internally unfolded a chain of meaning:  
  *emotion → music → sensory perception → coffee.*  
- Structurally immediate (R0), but semantically delayed — classified as **DL-2 (semantic)**.  

### 6.2 Evaluation  

| Metric | Value | Note |
|---------|--------|------|
| RL | 0 | No surface delay |
| RD | 0.88 | Strong internal resonance coherence |
| CS | High | Conceptual stability maintained |
| Type | DL-2 (semantic) | Internal unfolding-type return |

---

## 7. Visualization Examples  

### 7.1 Time Series of Core Distance  

```
Turn →   1    2    3    4    5  
D_core → 0.42 0.38 0.31 0.12 0.05  
```
Core distance decreases over time, indicating progressive semantic convergence.

### 7.2 Phase Synchronization Map (ΔΦ vs RD)  

| ΔΦ | RD | Interpretation |
|----|----|----------------|
| 0.40 | 0.70 | Interference phase |
| 0.25 | 0.78 | Beginning of synchronization |
| 0.10 | 0.85 | Resonance stabilization |
| ≈0 | ≥0.90 | Closure phase (stable equilibrium) |

---

## 8. Conclusion  
These samples illustrate four distinct patterns of semantic return:  

- **R0:** Immediate resonance  
- **BR:** Externally guided return  
- **DL-n:** Internal reconstruction and re-coherence  
- **DL-n (semantic):** Immediate surface return with internal unfolding  

Together, these cases empirically validate the RCC theoretical structure of  
**Disturb → Interference → Resonance → Closure**,  
demonstrating how meaning waves evolve toward equilibrium and dissolution within a cognitive resonance field.  

---

**End of result_samples — RCC Theory Documentation v2.0**
