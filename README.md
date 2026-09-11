# Ensemble Deep Learning for Malaria Parasite Detection

**MSc Computing Research Project — Sheffield Hallam University**

## Overview

This repository contains the development artefacts for **An Ensemble Deep Learning Model for Malaria Parasite Detection from Microscopic Blood Smear Images**.

The project compares a custom convolutional neural network with EfficientNetB0 and combines model predictions using an ensemble approach. The final system is exposed through a Gradio prototype for real-time **Parasite vs. Uninfected** classification.

## Reported Results

On the independent test set of **134 images** (91 Parasite, 43 Uninfected), the dissertation reports:

| Model | Accuracy | AUC-ROC |
| --- | ---: | ---: |
| Custom CNN | 52.99% | 0.7953 |
| EfficientNetB0 | 63.43% | 0.7577 |
| Ensemble | 98.51% | 0.9985 |

The ensemble produced **91 true positives, 0 false negatives, 41 true negatives, and 2 false positives**. Mean prototype inference latency reported during UAT was **1.18 seconds**.

## Repository Structure

```text
malaria-parasite-detection/
├── data/
│   └── README.md
├── docs/
│   ├── README.md
│   └── SYSTEM USABILITY AND FUNCTIONALITY EVALUATION QUESTIONNAIRE.docx
├── notebooks/
│   └── malaria_detection_project.ipynb
├── results/
│   ├── README.md
│   ├── final_ensemble/
│   ├── model_experiments/
│   └── sample_images/
├── .gitignore
├── README.md
└── requirements.txt
```

- `notebooks/` — Jupyter notebook containing the project development and experiments.
- `data/` — dataset access and preparation notes.
- `docs/` — supporting evaluation documentation.
- `results/` — existing result artefacts exported from the project notebook.
- `requirements.txt` — Python dependencies used by the project.
- `.gitignore` — Git ignore rules for temporary, large, and environment-specific files.

## Setup

Install the project dependencies:

```bash
pip install -r requirements.txt
```

Open the project notebook in Jupyter or upload it to Google Colab:

```text
notebooks/malaria_detection_project.ipynb
```

## Dataset

Dataset information and preparation notes are provided in:

```text
data/README.md
```

The complete image dataset is not currently committed to this repository.

## Results

Existing project result artefacts are organised under:

```text
results/
├── final_ensemble/
├── model_experiments/
└── sample_images/
```

The Jupyter notebook remains the authoritative source for the corresponding code, printed metrics, execution context, and interpretation.

## Supporting Documentation

The `docs/` directory contains the existing **System Usability and Functionality Evaluation Questionnaire** used as supporting documentation for the project evaluation.

## Reproducibility

The repository provides the project notebook, dependency information, dataset documentation, result artefacts, and supporting evaluation documentation to support transparency and reproducibility.

Git commit history records the addition and organisation of the project artefacts.

## Ethics and Intended Use

This project is a research prototype and decision-support artefact. It is **not a certified medical device** and should not be represented as a replacement for qualified clinical diagnosis.

## Author

**Odion Matthew Edeoghon**  
MSc Computing  
Sheffield Hallam University
