# Hurricane Harvey Damage Classification

Deep-learning computer-vision project for classifying post-Hurricane Harvey satellite imagery as **damaged** or **non-damaged**.

## Project overview

This project was developed as undergraduate research in Computer Science & Business Systems at SRM Institute of Science and Technology. The work investigated whether convolutional neural networks could support faster post-disaster damage assessment from satellite imagery.

The repository preserves the original experimental notebook and the resulting research paper.

## Problem

Manual post-disaster damage assessment can be time- and labour-intensive. The project frames damage assessment as a binary image-classification problem:

- **Damaged**
- **Non-damaged**

## Approach

The original workflow included:

1. Preparing labelled Hurricane Harvey imagery.
2. Splitting images into training, validation and testing workflows.
3. Image preprocessing / augmentation with Keras `ImageDataGenerator`.
4. Training and comparing multiple convolutional neural-network architectures.
5. Evaluating performance using classification metrics and ROC/AUC analysis.

Architectures explored in the project included:

- Custom CNN architecture (CM1)
- Custom CNN architecture (CM2)
- VGG16-style architecture
- AlexNet-style architecture

The notebook also contains additional experimentation associated with the original research process.

## Technology

- Python
- TensorFlow / Keras
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter / Google Colab

## Evaluation

The project compared models using metrics including:

- Accuracy
- Precision
- Recall
- F1 score
- Confusion-matrix analysis
- ROC / AUC

The published paper reports the highest classification accuracy at approximately **93%** for the best-performing custom CNN model. The paper also reports that AlexNet produced the highest F1 score among the four compared models.

## Repository structure

```text
.
├── README.md
├── requirements.txt
├── notebooks/
│   └── original_experiments.ipynb
└── docs/
    └── published_paper.pdf
```

## Reproducibility

The repository preserves the original code and research outputs, but the original image files used during the undergraduate project are not included.

The notebook was originally developed in Google Colab and contains historical Google Drive paths from the original training workflow. These paths will need to be replaced before rerunning the notebook in a new environment.

The original notebook references the Hurricane Harvey satellite-image dataset used during the project. Because the exact original local copy is no longer retained, the reported results in this repository should be treated as preserved experimental results rather than a claim that a fresh clone will reproduce the metrics without additional dataset setup.

## Research publication

The repository includes the paper **“Hurricane Disaster Mitigation by Processing Landscape Images”**, co-authored as part of the undergraduate project.

## Limitations

- Binary classification simplifies the broader problem of disaster-damage assessment.
- The original dataset is not bundled with this repository.
- The notebook reflects an undergraduate experimental workflow rather than a production ML pipeline.
- Reported metrics are those produced during the original project and documented in the accompanying research paper.

## Why this repository exists

This repository packages the original research work into a transparent portfolio artifact. It preserves the implementation and documented results while clearly separating the historical experimental environment from a production-ready ML system.
