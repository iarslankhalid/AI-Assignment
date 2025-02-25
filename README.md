##  Proposed Project Structure

```bash
AI_Assignment/
│
├── data/                      # Datasets for classification and clustering
│   ├── raw/                   # Raw datasets
│   ├── processed/             # Preprocessed datasets
│
├── notebooks/                 # Jupyter notebooks for EDA and experimentation
│   ├── classification_eda.ipynb
│   ├── clustering_eda.ipynb
│
├── src/                       # Source code
│   ├── __init__.py
│   ├── data_preprocessing/
│   │   ├── __init__.py
│   │   ├── preprocess_spam.py        # Preprocessing for spam dataset
│   │   └── preprocess_anomaly.py     # Preprocessing for anomaly detection dataset
│   │
│   ├── models/
│   │   ├── __init__.py
│   │   ├── cnn_classifier.py         # CNN for spam detection
│   │   ├── bayes_classifier.py       # Bayes Classifier for spam detection
│   │   ├── kmeans_clustering.py      # K-Means for anomaly detection
│   │   └── knn_clustering.py         # KNN for anomaly detection
│   │
│   ├── evaluation/
│   │   ├── __init__.py
│   │   ├── evaluate_classification.py # Evaluation metrics for classification
│   │   └── evaluate_clustering.py     # Evaluation metrics for clustering
│   │
│   └── utils/
│       ├── __init__.py
│       └── helpers.py                # Utility functions (e.g., plotting, data loading)
│
├── experiments/               # Scripts for running full experiments
│   ├── run_classification.py
│   └── run_clustering.py
│
├── results/                   # Results, plots, confusion matrices, etc.
│
├── reports/                   # Final report and intermediate summaries
│   └── figures/               # Figures to be included in the report
│
├── tests/                     # Unit tests for modules
│   ├── test_preprocessing.py
│   ├── test_models.py
│   └── test_evaluation.py
│
├── requirements.txt           # Python dependencies
├── README.md                  # Project overview and instructions
└── .gitignore                 # Git ignore file
```