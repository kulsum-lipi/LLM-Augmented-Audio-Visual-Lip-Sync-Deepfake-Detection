# Lip-Sync Deepfake Detection

This repository contains the full workflow for detecting lip-sync deepfakes in audio-visual content using a combination of **SyncNet scores**, **phoneme/viseme drift analysis**, and **LLM-based consistency checks**. The project is organized as a **day-wise iterative study** (Day 1–10) covering dataset collection, preprocessing, model training, evaluation, and analysis.

---

## Project Overview

The goal of this project is to develop a robust pipeline for **lip-sync deepfake detection**, integrating multiple modalities:

- **Visual features:** SyncNet, AV-HuBERT embeddings  
- **Audio features:** Phoneme/viseme alignment, drift computation  
- **LLM analysis:** Semantic and prosody consistency scoring  
- **Fusion modeling:** Combines all scores into a final detection model  
- **Evaluation:** AUC/EER metrics, IoU for segment-level detection, ablation studies, and noise/compression tests

---

## Repository Structure

Top-level deliverables and folders:

/deliverables  
├── docs/          # Day-wise PDFs documenting experiments and findings  
│   ├── day1  
│   ├── day2  
│   ├── day3  
│   ├── day4  
│   ├── day5  
│   ├── day6  
│   ├── day7  
│   ├── day8  
│   └── day9  
├── model/         # Trained fusion model (fusion_model.pkl)  
├── notebooks/     # Colab notebooks for all experiments   
├── visuals/       # Figures: plots, timelines, ablation tables  
└── README.md      # Project overview and usage instructions

---

## Day-wise Summary

| Day | Highlights |
|-----|------------|
| **1** | Pilot clip selection, preprocessing policy, feature plan, LLM scoring spec, error taxonomy, demo checklist |
| **2** | Dataset setup, baseline model run, evaluation metrics |
| **3** | Feature cache (SyncNet/AV-HuBERT), MFA phoneme timings, schema, LLM prompt templates |
| **4–5** | Phoneme timings, viseme/phoneme drift computation, LLM scores |
| **6** | Fusion model training, AUC/EER evaluation, model saved |
| **7** | Segment-level scoring, IoU calculation, example timelines |
| **8** | Noise/compression robustness, ablation study, lessons captured |
| **9** | Error analysis page, plots, short result summary |


---
