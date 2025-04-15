# Extracted and Analyzed EEG Features

## 1. Sample Entropy

- EEG is complex and non-linear—SampEn captures dynamics that mean or power measures might miss.
- **SampEn(m, r, N)** measures unpredictability by comparing pattern matches of length `m` vs. `m + 1`.
- Let:
  - `A` = matches for length `m + 1`
  - `B` = matches for length `m`
  - Then: **SampEn = –ln(A / B)**
- More drop in matches = more irregular signal = higher entropy (less predictable).
- **Interpretation:**
  - Higher SampEn → erratic brain activity → related to **anxiety**
  - Lower SampEn → stable patterns → related to **relaxation**

---

## 2. Event-Related Potentials (ERP) and Their Relation to Anxiety
*From: `ERP_Coherence.ipynb`*

### ◼ N200
- **Latency:** 200–350 ms  
- **Electrode Sites:** FCz, Cz  
- **Function:** Reflects conflict monitoring and cognitive control.  
- **Anxiety Link:**  
  - Enhanced N200 amplitudes in anxious individuals, especially during conflict/error tasks (e.g., Stroop, Flanker).
  - *PMC4033096*: Shows stronger cognitive control engagement in early stages in anxious individuals.

### ◼ P300
- **Latency:** 300–500 ms  
- **Electrode Sites:** Pz  
- **Function:** Attention allocation and stimulus significance evaluation.  
- **Anxiety Link:**  
  - Reduced P300 amplitude in high-anxiety individuals → impaired attentional resource allocation.
  - *PubMed 20374540*: Blunted P300 responses in tasks involving stimulus discrimination and decision-making.

### ◼ FRN (Feedback-Related Negativity)
- **Latency:** 250–350 ms  
- **Electrode Sites:** FCz, Cz  
- **Function:** Feedback processing; evaluation of negative outcomes or errors.  
- **Anxiety Link:**  
  - Increased FRN amplitude in anxious individuals → heightened sensitivity to negative feedback or perceived failure.

---

## 3. Phase-Amplitude Coupling (PAC): Theta–Alpha, Theta–Beta, Theta–Gamma

*From: `Phase_Amplitude_Coupling.ipynb`*

- PAC examines how slow theta waves influence the strength (amplitude) of faster waves (alpha, beta, gamma).
- Analogy: Slow theta waves set a rhythm, faster waves (alpha/beta/gamma) follow it.
- This coordination enables efficient communication between brain regions.
- **Anxiety Link:**
  - In high trait anxiety, PAC patterns change—especially in how theta affects fast rhythms tied to **attention** and **emotion**.
  - PAC is useful for capturing cross-frequency coupling → helps predict anxiety levels from EEG.

---

## 4. Alpha Frontal Coherence

*From: `ERP_Coherence.ipynb`*

- **Coherence** quantifies how consistently two EEG channels oscillate together (0 = no sync, 1 = perfect sync).
- Focus on **Alpha band (8–12 Hz)** → associated with **relaxation**, **attention**, and **emotional regulation**.
- **Frontal regions:** F3, F4, Fz  
- Calculated alpha-band coherence between frontal channels to assess functional connectivity related to anxiety and cognitive control.

---
