# Lung Cancer Detection via Cough Spectrograms

This project detects **lung cancer and other respiratory diseases** from **cough audio recordings** by converting them into **Log-Mel spectrograms** and training deep learning models (ResNet, Audio Spectrogram Transformer).

## Project Overview
- Converts `.wav` cough recordings into **256×256 spectrogram images**.
- Trains a **ResNet-18 baseline (Proof of Concept)** for binary classification (healthy vs cancer).
- Plans to scale to:
  - **ResNet-50** for improved accuracy.
  - **AST (Audio Spectrogram Transformer)** with PEFT for multi-class classification.

## Repo Structure
```
data/               - Processed and raw datasets
models/             - Saved trained models
notebooks/          - Jupyter Notebooks (PoC workflow)
scripts/            - Utility scripts for preprocessing and training
outputs/            - Results (plots, confusion matrices)
```

## Quick Start
1. Clone the repo:
```bash
git clone https://github.com/saudAbd/lung-cancer-cough-classification.git
cd lung-cancer-cough-classification
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run Jupyter Notebook:
```bash
jupyter notebook notebooks/01_PoC_ResNet18.ipynb
```

## Next Steps
- Prepare **full binary dataset** (3,600+ samples) with train/val/test split.
- Train **ResNet-50** and **AST (Audio Spectrogram Transformer)** with PEFT.
- Expand to **multi-class classification** (Pneumonia, COVID-19, etc.).

## Author
**Saud Abdullah** – MSc Computer Science, 2025.
#   l u n g - c a n c e r - c o u g h - c l a s s i f i c a t i o n  
 