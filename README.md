# Local Transport Mixtures for Zero-Shot Voice Conversion in SSL Spaces — Audio Demonstrations

Official demonstration website for the paper:  
**"Local Transport Mixtures for Zero-Shot Voice Conversion in SSL Spaces"** *(Under Review)*.

**Authors:** Samir Sadok, Xavier Alameda-Pineda  
*Inria, Univ. Grenoble Alpes, CNRS, Grenoble INP, LJK, France*

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

1. **Curated Voice Conversion Benchmark (9 Pairs)**:
   - Comprehensive cross-gender and same-gender conversions ($F \to M$, $M \to F$, $F \to F$, $M \to M$).
   - Ground truth Source & Target reference audios.
   - Side-by-side comparison of **Proposed LWT ($\alpha=1.5$)** against:
     - Standard LWT ($\alpha=1.0$)
     - LinearVC (Interspeech 2025)
     - kNN-VC ($k=4$, IEEE TASLP 2023)
     - Classic Global WCT
   - Dynamic vector SVG waveform players with time seeking and real-time playback progress.

2. **Neutral Voice Conversion (Canonical Gender-Balanced Voice)**:
   - Conversion to a speaker-invariant neutral voice by projecting onto a gender-neutral universal background model (UBM) trained on 40 speakers (20 Males / 20 Females strictly 50/50 balanced).
   - Audio comparisons across 4 diverse speakers (Male & Female) showing collapse into the canonical neutral voice (~160 Hz) with **0.00% Character Error Rate (CER)**.

3. **Unified Objective Benchmark Summary ($N=200$)**:
   - Comprehensive quantitative comparison across 200 conversions on LibriSpeech `test-clean`:
     - Intelligibility (Wav2Vec2 CER/WER, Whisper CER)
     - Speaker Similarity (ECAPA-TDNN cosine similarity)
     - Naturalness (UTMOS MOS)
     - Prosody preservation (Pitch correlation $r_{F_0}$, Loudness correlation $r_{\text{loudness}}$)
     - Computational speed (Real-Time Factor RTF)

4. **Code & Quickstart**:
   - Instructions and snippets for Python API and CLI (`boosted-lwt`).

---

## 💻 Code Repository

The complete Python package, CLI tools, and reproducible evaluation code can be found in the main repository:  
🔗 **[Local Transport Mixtures Code Repository](https://github.com/<your-username>/boosted-lwt)**

---

## 📄 Citation

```bibtex
@article{sadok2026local,
  title     = {Local Transport Mixtures for Zero-Shot Voice Conversion in SSL Spaces},
  author    = {Sadok, Samir and Alameda-Pineda, Xavier},
  journal   = {Under Review},
  year      = {2026}
}
```

