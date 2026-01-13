**Project Overview**
High-dimensional datasets often suffer from the "Curse of Dimensionality," containing redundant, noisy, or irrelevant features that increase computational complexity and degrade model performance.

This project implements a robust pipeline for Unsupervised Feature Selection and Cluster-Based Feature Reduction. Since real-world data is often unlabeled, this project focuses on extracting the most informative features based purely on the intrinsic mathematical structure of the data.

**Objectives**
The core goal is to transform a "noisy" high-dimensional dataset into a compact, high-value feature set using:

Variance Thresholding: Eliminating constant or low-information attributes.

Correlation-Based Filtering: Removing redundant features that share linear dependencies.

Cluster-Based Reduction: Grouping similar features and selecting a "representative" from each cluster based on variance and mean correlation.

Non-Linear Embedding: Utilizing Autoencoders and t-SNE for advanced visualization and reduction.


**Methodology**
Data Preprocessing: Cleaning missing values and standardizing features.

EDA: Visualizing distributions and pairwise correlations.

Unsupervised Selection: * Applying VarianceThreshold.

Constructing a Correlation Matrix to drop redundant pairs.

Feature Clustering: Treating features as data points and using Hierarchical/K-Means clustering to find feature families.

Selection Criteria: Choosing the "Best Representative" from each cluster using Highest Variance or Highest Mean Correlation.

Comparison: Evaluating the reduced dataset against the original structure.

**Future Scope**
Hybrid Pipelines: Combining unsupervised reduction with supervised validation (LASSO/Random Forest).

Deep Learning: Implementing Transformer-based feature embeddings.

Scalability: Optimizing for Big Data using parallel computing.
