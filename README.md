# Robust Voice Activity Detection for Distant and Noisy Speech

**A Comparative Study of Classical and Neural Methods on the VOiCES Corpus**

**Student:** Abdulameer Farhan Aljmmali  
**Student ID:** 404131110  
**Course:** Speech and Audio Processing

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/amiralgmaly-glitch/vad-voices-research/blob/main/VAD_VOiCES_Comparison_Abdulameer_Aljmmali.ipynb)

## Project files

| File | Description |
| --- | --- |
| [Research paper (PDF)](VAD_VOiCES_Paper_Abdulameer_Aljmmali.pdf) | Full paper: method, experiments, results and discussion |
| [Presentation (PowerPoint)](VAD_VOiCES_Presentation_Abdulameer_Aljmmali.pptx) | 14 slides with speaker notes |
| [Code (Jupyter Notebook)](VAD_VOiCES_Comparison_Abdulameer_Aljmmali.ipynb) | All experiments, with results and figures |

## Summary

Five Voice Activity Detection (VAD) methods are compared on distant, noisy speech from the VOiCES corpus:

1. Energy-based detector
2. WebRTC VAD
3. Silero VAD (pre-trained neural model)
4. MFCC features + gradient boosting
5. Spectrogram CNN

## Results

| System | Precision | Recall | F1 |
| --- | --- | --- | --- |
| Energy | 0.922 | 0.972 | 0.946 |
| WebRTC VAD (mode 2) | 0.874 | 0.981 | 0.924 |
| Silero VAD | 0.911 | 0.978 | 0.944 |
| MFCC + boosting | 0.914 | 0.984 | 0.948 |
| **Spectrogram CNN** | **0.931** | 0.977 | **0.953** |

## How to run

Open the notebook in Google Colab and choose **Runtime -> Run all**. The VOiCES data is downloaded automatically from the public AWS bucket `lab41openaudiocorpus`.

## Tools

Python, librosa, scikit-learn, PyTorch, webrtcvad, silero-vad, Google Colab.
