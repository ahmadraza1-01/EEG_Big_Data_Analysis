Features we extracted and analysed: 
1. Sample Entropy
→ EEG is complex and non-linear—SampEn captures dynamics that mean or power measures might miss.
→ SampEn(m, r, N) measures unpredictability by comparing pattern matches of length m vs. m + 1.
→ A = matches for length m + 1, B = matches for length m → SampEn = –ln(A/B).
→ More drop in matches = more irregular signal = higher entropy (less predictable)..
→ Higher SampEn = erratic brain activity - related to anxiety; Lower SampEn = stable patterns - related to relaxation

2. Event Related Potential and their relation to anxiety
ERP_Coherence.ipynb
N200
Latency: 200–350 ms
Electrode Sites: FCz, Cz
Function: Reflects conflict monitoring and cognitive control.
Anxiety Link: Studies show enhanced N200 amplitudes in anxious individuals, particularly in tasks involving conflict or error detection (e.g., Stroop or Flanker tasks).
  PMC4033096 notes that anxious individuals show stronger cognitive control engagement in early processing stages.

P300
Latency: 300–500 ms
Electrode Sites: Pz
Function: Related to attention allocation and evaluation of stimulus significance.
Anxiety Link: Reduced P300 amplitude is consistently observed in high-anxiety individuals, suggesting impaired attentional resource allocation or difficulty in processing uncertainty.
  PubMed 20374540 reports blunted P300 responses in anxious subjects during tasks requiring stimulus discrimination and decision-making.

FRN (Feedback-Related Negativity)
Latency: 250–350 ms
Electrode Sites: FCz, Cz
Function: Signals the brain's evaluation of negative outcomes or errors (feedback processing).
Anxiety Link: FRN amplitude is increased in anxious individuals, reflecting a heightened sensitivity to negative feedback or perceived failure

3. Theta alpha, Theta beta, Theta gamma coupling (Phase Amplitude Coupling)
Phase_Amplitude_Coupling (PAC).ipynb

Phase–Amplitude Coupling (PAC) looks at how theta waves (slow) influence the strength of faster brain waves (like alpha, beta, or gamma). It’s like the slow waves set the rhythm, and the fast waves follow along with more or less activity depending on where they are in the slow wave's cycle. This coordination helps different parts of the brain work together more efficiently. In people with higher trait anxiety, this coordination can be different—especially in how theta waves affect faster waves linked to attention and emotion. Because PAC captures how brain areas communicate over time, it can be a useful and sensitive feature to help understand and predict anxiety levels from EEG data.

4. Coherence_alpha_frontal:
ERP_Coherence.ipynb
Coherence measures the functional connectivity between two EEG channels by quantifying how consistently they oscillate together at each frequency. It ranges from 0 (no synchrony) to 1 (perfect synchrony). Alpha band (8–12 Hz) is often linked with relaxation, attention, and anxiety-related changes.Frontal regions (F3, F4, Fz) are important in emotional regulation, attention, and cognitive control. alpha-band coherence values between frontal channels is calculated


Group Members: 
1) Ahmad Raza - 220088
2) Anya Rajan - 220191
3) Debarpita Dash - 220328
4) Manasvi Nidugala - 220613
5) Nischay Patel - 220721
6) Poojal Katiyar - 220770
