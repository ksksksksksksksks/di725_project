# Multi-Modal Transformer for Text-Conditioned Land Cover Segmentation

METU DI-725 – Spring 2026 term project

This repository contains the code for a three-phase study on integrating textual descriptions into SegFormer-B0 for land cover segmentation.

## Overview

- **Phase 1 (Proof of Concept):** simple additive fusion of CLIP visual features and Sentence-BERT text embeddings, trained on a small subset.
- **Phase 2 (Full Benchmark):** FiLM-based conditioning of the SegFormer decoder with captions from five different sources (text-only, vision-only, hybrid), trained on the entire DI725 dataset.
- **Phase 3 (Ablation Study):** evaluating the same best multi-modal model on shuffled captions to prove that the model truly relies on textual information; reporting per-class IoU drop and confirming the importance of caption quality.

## Key Files

- `di725_poc.ipynb` – **initial feasibility experiment (proof of concept)**
- `di725-ph_2.ipynb` – **Phase 2 benchmark notebook (full multi-modal training)**
- `di725_ph3_ablation.ipynb` – **Phase 3 ablation study (shuffled captions, mIoU comparison, final plots)**
- `report_final.pdf` – **final project report (4 pages, includes all phases)**

## Links

- **W&B dashboard:** [here](https://wandb.ai/e278979-metu-middle-east-technical-university/di725-project/workspace?nw=gj32ledushe)  
  (training curves, per-class IoU, experiment tracking, ablation metrics)
- **Project reports:** `report_phase1.pdf`, `report_phase2.pdf`, `report_final.pdf`

## Dataset

The dataset comprises RGB images, pixel-level segmentation masks (7 classes), and automatically generated captions. The dataset is **not** included in this repository due to licensing restrictions.
