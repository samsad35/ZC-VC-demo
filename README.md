# Boosted Local Wasserstein Transport (Boosted LWT) — Audio Demonstrations

Official demonstration website for the paper:  
**"Boosted Local Wasserstein Transport: Zero-Shot Voice Conversion via Closed-Form Optimal Transport and Analytical Speech Disentanglement in Self-Supervised Spaces"** *(ICASSP 2026 Submission)*.

---

## 🌐 Live Online Demo (GitHub Pages)

You can host this website directly using **GitHub Pages**:
1. Push this repository to GitHub (e.g. `https://github.com/<your-username>/boosted-lwt-demo`).
2. Go to repository **Settings** &rarr; **Pages**.
3. Under **Build and deployment** &rarr; **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. Within a few minutes, your site will be live at:
   ```
   https://<your-username>.github.io/boosted-lwt-demo/
   ```

---

## 🎧 What's Inside This Demonstration

1. **Analytical Speech Disentanglement (Pure Content Extraction)**:
   - Demonstration of extracting speaker-invariant phonetic content by projecting onto a gender-neutral universal background model (UBM) trained on 40 speakers (20 Males / 20 Females strictly 50/50 balanced).
   - Audio comparisons across 4 diverse speakers (Male & Female) showing collapse into the canonical neutral voice (~160 Hz) with **0.00% Character Error Rate (CER)**.

2. **Benchmark Voice Conversion (9 Curated Pairs)**:
   - Comprehensive cross-gender and same-gender conversions ($F \to M$, $M \to F$, $F \to F$, $M \to M$).
   - Ground truth Source & Target reference audios.
   - Side-by-side comparison of **Boosted LWT ($\alpha=1.5$)** against:
     - Local Wasserstein Transport (LWT $\alpha=1.0$)
     - LinearVC (Interspeech 2025)
     - kNN-VC ($k=4$, IEEE TASLP 2023)
     - Classic Global WCT
   - Dynamic vector SVG waveform players with time seeking and real-time playback progress.

3. **Unified Objective Benchmark Summary ($N=200$)**:
   - Comprehensive quantitative comparison across 200 conversions on LibriSpeech `test-clean`:
     - Intelligibility (Wav2Vec2 CER/WER, Whisper CER)
     - Speaker Similarity (ECAPA-TDNN cosine similarity)
     - Naturalness (UTMOS MOS)
     - Prosody preservation (Pitch correlation $r_{F_0}$, Loudness correlation $r_{\text{loudness}}$)
     - Computational speed (Real-Time Factor RTF)

---

## 💻 Code Repository

The complete Python package, CLI tools, and reproducible evaluation code can be found in the main repository:  
🔗 **[Boosted LWT Code Repository](https://github.com/<your-username>/boosted-lwt)**

---

## 📄 Citation

```bibtex
@inproceedings{boosted_lwt_icassp2026,
  title     = {Boosted Local Wasserstein Transport: Zero-Shot Voice Conversion via Closed-Form Optimal Transport and Analytical Speech Disentanglement in Self-Supervised Spaces},
  author    = {Anonymous Authors},
  booktitle = {IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  year      = {2026}
}
```
