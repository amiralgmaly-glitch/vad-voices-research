# Robust Voice Activity Detection for Distant and Noisy Speech

**A Comparative Study of Classical and Neural Methods on the VOiCES Corpus**

**Student:** Abdulameer Farhan Aljmmali  
**Student ID:** 404131110  
**Course:** Speech and Audio Processing

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/amiralgmaly-glitch/vad-voices-research/blob/main/VAD_VOiCES_Comparison_Abdulameer_Aljmmali.ipynb)

This repository contains the code for the research project. It compares five Voice Activity Detection (VAD) methods on distant, noisy speech from the VOiCES corpus:

1. Energy-based detector
2. WebRTC VAD
3. Silero VAD (pre-trained neural model)
4. MFCC features + gradient boosting
5. Spectrogram CNN

Results are reported as frame-level (30 ms) precision, recall and F1, broken down by background noise (none, babble, music, television), microphone distance and room, on a speaker-independent test split.

## How to run
Open the notebook in Google Colab and choose **Runtime -> Run all**. The VOiCES data is downloaded automatically from the public AWS bucket `lab41openaudiocorpus`.

## Tools
Python, librosa, scikit-learn, PyTorch, webrtcvad, silero-vad, Google Colab.
