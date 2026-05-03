# Multi-Modal Transformer for Text-Conditioned Land Cover Segmentation

METU DI-725 – Spring 2026 term project

This repository contains the code for a two-phase study on integrating textual descriptions into SegFormer-B0 for land cover segmentation.

## Overview

- **Phase 1 (Proof of Concept):** simple additive fusion of CLIP visual features and Sentence-BERT text embeddings, trained on a small subset.
- **Phase 2 (Full Benchmark):** FiLM-based conditioning of the SegFormer decoder with captions from five different sources (text-only, vision-only, hybrid), trained on the entire DI725 dataset.

## Key Files

- `phase1_proof_of_concept.ipynb` – initial feasibility experiment
- `di725-ph_2.ipynb` – **latest and final version of the Phase 2 benchmark notebook**

> ⚠️ Due to naming issues, the Phase 2 notebook may also appear under older filenames such as `phase2_benchmark.ipynb` or `di725_bench.ipynb`. Always use `di725-ph_2.ipynb` for the final results.

## Links

- **W&B dashboard:** [here]([https://wandb.ai/ksen1a-princeton-university/METUCENG501](https://wandb.ai/e278979-metu-middle-east-technical-university/di725-project/workspace?nw=gj32ledushe))  
  (training curves, per-class IoU, experiment tracking)
- **Project reports:** included in the repository as `report_ph?.pdf`

## Dataset

The dataset comprises RGB images, pixel-level segmentation masks (7 classes), and automatically generated captions. The dataset is **not** included in this repository due to licensing restrictions.
