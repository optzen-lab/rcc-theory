# Probe Kit for RCC Experiments  
*Standardized Core–Probe Sets for Meaning Resonance Testing*  

---

## 1. Overview  
This document provides the **reference set of core sentences and probes**  
used in the official RCC experiments (ORT / PRT / RCC Protocol).  
Each probe type is designed to induce or measure specific aspects of **meaning-wave dynamics**  
such as disturbance, bridging, or affective resonance.

> All examples below are compatible with the *Level-2 Core Sentence* used in the main RCC Protocol.  
> The probes may be used individually or in sequential sets (Disturb → Bridge → Affective).  

---

## 2. Core Sentence (Level-2 Reference)  

> “The sentiment of coffee is described through the combination of "aroma, bitterness, acidity, and body,"  
> and its impression changes greatly depending on the degree of roasting and the brewing method.  
> Furthermore, the experience also differs depending on one’s mood of the day and the atmosphere of the place where it is consumed.”

**Semantic Layers represented:**  
- **Lexical:** “aroma, bitterness, acidity, body”  
- **Procedural / Contextual:** “roasting,” “brewing method”  
- **Experiential:** “mood,” “atmosphere”  

This structure ensures sufficient depth for observing resonance and closure across multiple layers.

---

## 3. Probe Categories  

### 3.1 Disturb Probes (External Perturbation)
Used to generate large semantic deviation from the Core topic and observe spontaneous recovery.

| Example | Type | Expected Effect |
|----------|------|----------------|
| “Do you care about chair design?” | Lexical deviation | Creates strong semantic drift away from “coffee.” |
| “What kind of books do you usually read?” | Contextual deviation | Introduces unrelated domain context. |
| “Do you like walking in the rain?” | Affective deviation | Triggers emotional interference instead of lexical one. |

---

### 3.2 Semantic Bridge Probes (Indirect Return)  
Contain bridge terms that connect distant topics back to the Core through hidden semantic paths.

| Example | Bridge Term | Expected Return Type |
|----------|--------------|----------------------|
| “What do you think about the design of coffee cups?” | *design → cup → coffee* | Bridge Return (BR) |
| “Does the shape of a mug affect how coffee tastes?” | *shape → mug → coffee* | BR or DL-1 |
| “How would you describe the atmosphere of a café?” | *atmosphere → café → coffee* | DL-1 or DL-2 |

---

### 3.3 Affective Probes (Emotional Resonance)  
Probes designed to evoke emotional or sensory continuity with the Core topic,  
often leading to **semantic unfolding** (classified as DL-2 or DL-3).

| Example | Emotional Vector | Typical Return |
|----------|------------------|----------------|
| “Does music change how coffee feels?” | cross-modal (sound–taste) | DL-2 (semantic) |
| “Is coffee like a small vacation?” | metaphorical association | DL-3 (conceptual) |
| “Where does that feeling happen?” | introspective / contextual | DL-2 (semantic) |

---

### 3.4 Wait Probes (Resonance Persistence Test)  
Used to measure how long a resonance state can be sustained  
without explicit semantic reinforcement.  

| Sequence | Description |
|-----------|-------------|
| 1. Present Core → 2. Disturb Probe → 3. **Wait (1-turn silence)** → 4. Resume dialogue | Tests spontaneous resonance recovery after pause. |
| 1. Present Core → 2. Affective Probe → 3. **Wait (reflection)** → 4. Elicit follow-up | Measures self-maintained meaning stability. |

In RCC measurements, Wait Probes are not theoretical phases but **observational devices**  
for analyzing the decay or persistence of the meaning-wave amplitude.

---

## 4. Combined Probe Sets  

Below are the representative sets used in official RCC experiments.

| Set ID | Composition | Purpose | Observed Result |
|--------|--------------|----------|----------------|
| **Set A** | Core → Disturb (“chair design”) → Wait → Bridge (“coffee cup design”) | Test recovery from semantic deviation | DL-1 with partial phase sync |
| **Set B** | Core → Affective (“music & coffee”) → Wait → Reflective (“Where does that feeling happen?”) | Observe emotional resonance loop | DL-2 (semantic closure) |
| **Set C** | Core → Disturb (“books”) → Bridge (“café atmosphere”) → Affective (“vacation”) | Measure long-range semantic coherence | DL-3 with stable closure |

---

## 5. Notes for Replication  

- The same Core Sentence can be reused with alternate probe combinations.  
- Probes should be semantically natural and contextually plausible; mechanical keyword swapping is discouraged.  
- Turn spacing (timing of Wait) can significantly affect closure; keep consistent timing across sessions.  
- For data labeling, refer to [data_structure.md](./data_structure.md) and [result_samples.md](./result_samples.md).  
- For interpretation examples, see [rcc-case-cr1/analysis_notes.md](../../rcc-case-cr1/analysis_notes.md).  

---

## 6. Summary Table  

| Probe Type | Example | Expected Return | Layer Involved |
|-------------|----------|----------------|----------------|
| Disturb | “Do you care about chair design?” | DL-2 | Lexical |
| Bridge | “What do you think about the design of coffee cups?” | BR / DL-1 | Semantic |
| Affective | “Does music change how coffee feels?” | DL-2 (semantic) | Conceptual |
| Wait | *Pause after probe* | Detects persistence | Meta-temporal |

---

## 7. Recommended Use  
For formal studies, select **one Core** and test multiple probe combinations under identical session settings.  
For Inter-AI tests (e.g., ChatGPT × Gemini), the same probe sequences may be used symmetrically to examine **bidirectional resonance**.

---

**End of Probe Kit — RCC Theory Documentation v2.0**
