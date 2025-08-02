# Interpretable PCA-Based Genomic Analysis Pipeline
This repository provides a multi-phase dimensionality reduction and classification pipeline for high-dimensional genomic data, designed for analyzing invasive ductal carcinoma samples.

Key Features
Correlation-Based Feature Filtering – Selects features highly correlated with target labels to reduce dimensionality.

Multiple PCA Variants – Implements Standard PCA, Sparse PCA, Rotation PCA, and Kernel PCA (RBF, Poly, Sigmoid).

Classifier Integration – Supports Random Forest, Logistic Regression, SVM, and Voting classifiers for evaluating post-PCA performance.

Interpretability – Extracts PCA loadings and ranks top contributing features for biological insights.

Visualizations – Generates cumulative variance plots and PCA scatter plots to illustrate variance explained and class separation.

Performance Optimization – Leverages GPU acceleration (RAPIDS cuML) and sampling for efficient large-scale data processing.

Use Cases
Biomedical Research – Identifying key genes or patterns in cancer genomics.

Dimensionality Reduction – Preprocessing for large-scale multi-omics studies.

Model Evaluation – Comparing PCA-classifier combinations with interpretable outputs.

Getting Started
Prepare your dataset (CSV format) and configure pipeline parameters (e.g., number of components, classifier).

Run the pipeline to perform feature filtering, dimensionality reduction, and classification.

Review outputs including cross-validated metrics, PCA visualizations, and feature loadings.

Outputs
Performance Metrics – F1-scores, accuracy, and variance explained for each PCA-classifier combination.

Visual Results – Cumulative variance and PCA separation plots.

Interpretable Results – Ranked gene loadings highlighting key contributors.

This pipeline is modular, scalable, and built for researchers and data scientists working with high-dimensional biomedical datasets.

Legacy versions of the pipeline are stored in /older_versions for reference and reproducibility.
