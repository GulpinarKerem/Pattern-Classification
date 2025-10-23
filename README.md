# Pattern-Classification
Pattern Classification project under Gerhard Widmer 

This repository contains experiments conducted for the MLPC 2025 challenge, focusing on multilabel classification of environmental audio clips. The project explores multiple machine learning approaches for classifying frame-level embeddings extracted from raw audio.

🔍 Project Overview

Each audio file is represented as a multilabel matrix of shape (58, 220, 1), covering 58 possible sound classes across temporal frames. The main goal is to build and evaluate robust classifiers capable of identifying multiple simultaneous sound events.

🧠 Methods

The project includes:

Data Labeling & Exploration – Assessment of annotation consistency and class diversity

Dimensionality Reduction – PCA applied to 768-D audio embeddings, preserving 95% of variance (184 components)

Data Splitting – File-level train/validation/test split (70/20/10) with leakage prevention

Classification Models –

k-Nearest Neighbors (k-NN)

Random Forest (RF)

XGBoost

Feedforward Neural Network

⚙️ Experiments & Evaluation

Data preprocessing: z-score normalization + PCA

Evaluation metrics: macro-averaged F1, ROC-AUC, balanced accuracy

Overfitting prevented via early stopping and dropout

Final model (Neural Network) achieved:

Accuracy: 0.954

F1 Score: 0.737

ROC AUC: 0.875

📊 Key Findings

Random Forest severely overfit and performed poorly on minority classes.

XGBoost showed strong potential but was limited by computational constraints.

k-NN provided a stable, interpretable baseline.

The Neural Network demonstrated the best generalization and robustness.

