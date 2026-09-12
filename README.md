# CSE715: Neural Networks and Fuzzy System


## GNN-BERT Music Context
This course project explores multimodal music understanding by combining textual metadata with the temporal structure of music. The project uses BERT-based representations, graph neural networks, multimodal fusion, and music captioning.


## Tasks
- **Task 1 -- BERT Baseline for Music Tag Understanding:** Uses track metadata and text with BERT to predict music-related tags from the MagnaTagATune dataset.
- **Task 2 -- GNN on Music Structure Graphs:** Represents the temporal structure of music as graphs and applies a graph attention network for genre classification.
- **Task 3 -- GNN–BERT Fusion for Multi-Context Understanding:** Combines textual BERT embeddings and structural GNN embeddings. The notebook compares GNN-only, BERT-only, Early Concat Fusion, and Cross-Attention Fusion models. It includes genre classification, evaluation metrics, confusion matrices, precision-recall curves, t-SNE visualizations, and qualitative graph analysis.
- **Task 4 -- Cross-Modal MusicCaps Alignment:** Explores music caption generation using the MusicCaps dataset and multimodal music representations.


## Dataset Used
- **FMA-small:** Audio files and metadata containing 8,000 30-second tracks across eight genres, used for genre classification and music structure graph construction.
- **MagnaTagATune:** Music clips, metadata, and human-annotated tags containing 25,863 annotated clips and 188 tags, used for multi-label music tag classification.
- **MusicCaps:** 5,521 music examples paired with natural-language captions describing the corresponding audio, used for audio--text representation learning and retrieval.


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
├── .gitignore
├── config.yaml
├── README.md
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


## Project Report
[Context-Aware Music Understanding Using Graph Neural Networks and BERT: A Multimodal Fusion Approach](report/CSE715_Project_Report.pdf)



## Project Members
- [Niloy Ahsan](https://github.com/niloyahsan1)
- [Chaity Rani Ghosh](https://github.com/chaityrg)

---