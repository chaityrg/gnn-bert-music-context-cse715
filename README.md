# CSE715: Neural Networks and Fuzzy System

## GNN-BERT Music Context

This course project explores multimodal music understanding by combining textual metadata with the temporal structure of music. The project uses BERT-based representations, graph neural networks, multimodal fusion, and music captioning.

## Tasks

### Task 1: BERT-Based Music Tag Prediction

Uses track metadata and text with BERT to predict music-related tags from the MagnaTagATune dataset.

Notebook: `notebooks/task1_BERT.ipynb`

### Task 2: Graph Neural Network for Music Structure

Represents the temporal structure of music as graphs and applies a graph attention network for genre classification.

Notebook: `notebooks/task2_GNN.ipynb`

### Task 3: BERT + GNN Fusion

Combines textual BERT embeddings and structural GNN embeddings. The notebook compares GNN-only, BERT-only, Early Concat Fusion, and Cross-Attention Fusion models.

It includes genre classification, evaluation metrics, confusion matrices, precision-recall curves, t-SNE visualizations, and qualitative graph analysis.

Notebook: `notebooks/task3_BERT+GNN.ipynb`

### Task 4: Music Captioning

Explores music caption generation using the MusicCaps dataset and multimodal music representations.

Notebook: `notebooks/task4_MusicCap.ipynb`

## Dataset Used

- **FMA-small:** Audio files and metadata used for music genre classification and structural graph construction.
- **MagnaTagATune:** Music clips, annotations, and tag information used for BERT-based music tag prediction and mood-related analysis.
- **MusicCaps:** Music-caption pairs used for the music captioning task.
- **Processed data:** Prepared text, labels, and other intermediate data used by the notebooks.

## Project Structure

```text
.
├── dataset/
│   ├── fma_metadata/        FMA metadata tables
│   ├── fma_small/           FMA-small audio files
│   ├── magnatagatune/       MagnaTagATune annotations and clip metadata
│   ├── musiccaps/           MusicCaps data
│   └── processed/           Processed training data
├── notebooks/
│   ├── task1_BERT.ipynb
│   ├── task2_GNN.ipynb
│   ├── task3_BERT+GNN.ipynb
│   ├── task4_MusicCap.ipynb
│   └── saved models/        Saved model checkpoints and feature caches
├── report/
│   └── CSE715_Project_Report.pdf
├── results/
│   ├── task1/               Task 1 results
│   ├── task2/               Task 2 results
│   └── task3/               Task 3 results
├── config.yaml
└── requirements.txt
```

## Evaluation Metrics

The fusion notebook reports:

- Accuracy
- Macro-F1
- Per-class precision, recall, and F1
- Multiclass macro AUC-PR
- Confusion matrices
- Precision-recall curves

The final results table is generated inside `task3_BERT+GNN.ipynb` after the model evaluation cells have completed.

## Report

The project report is available at [report/CSE715_Project_Report.pdf](report/CSE715_Project_Report.pdf).

## Current Status

This repository is an ongoing course project. `config.yaml`, `requirements.txt`, `results/`, and any missing script-based entry points should be treated as work in progress; the notebooks are the current source of truth for the experiments.