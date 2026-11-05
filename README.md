# Comparing Surface Code Decoders in Stim
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vnx45_SdjgiFhcHaNFPQBrWBVw-v7FM3#scrollTo=SWyKUGHdDuLy)

This repository introduces stim and uses it to compare the thresholds and runtimes of MWPM (minimum weight perfect matching) and BPOSD0 (belief propagation with order zero ordered statistics decoding) on small (rotated) surface codes.  It finds similar thresholds and drastically faster runtimes for MWPM.  

---

## Technical Highlights
* **Surface Code Tasks**: Uses Stim and Sinter to efficiently sample the surface code under circuit level noise for a variety of code distances and noise probabilities.
* **MWPM**: Uses PyMatching to decode using MWPM.  Using the data for a variety of noises and distances, finds a threshold of about a percent.  Also includes an introduction to MWPM.
* **BPOSD0**: Uses stimbpsd to decode using zeroth order BPOSD.  Using the data for a variety of noises and distances, finds a threshold of about a percent.  Also includes an introduction to BPOSD0.
* **Runtime Comparison**: Compares per shot latency of MWPM and BPOSD to find speedup of at least 78x using MWPM.   

---

## How to Run
This project is completely self-contained and designed to run directly in the cloud via Google Colab.

1. Click the **Open in Colab** badge at the top of this file.
2. Run the cells sequentially.
