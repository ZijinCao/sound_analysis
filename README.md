# Code Repository Overview

This repository contains code used for the computational analysis of sounds in our dataset, as described in our thesis. The analysis involves two main sets of code: one for extracting features using the Freesound API extractor and another for statistical analysis and correlating features with semantic descriptors.

## 1. Freesound API Extractor

For the computational analysis of sounds in our dataset, we employed the Freesound API extractor, grounded in Essentia. This tool can extract a foundational set of 91 primary low- and mid-level descriptors, including temporal aspects, spectral characteristics, spectro-temporal features, rhythmic elements, and tonal attributes. For more detailed descriptions of these descriptors, please refer to the [Freesound API analysis documentation](https://freesound.org/docs/api/analysis_docs.html#contents).

## 2. Statistical Analysis

Our analysis proceeds with two main stages aimed at clarifying how sound parameters relate to semantic descriptors: statistical analysis of features and feature importance ranking.

### (1) Statistical Analysis of Features

We assessed the normality of the distribution of these features using the Shapiro-Wilk test. Approximately 85% of the descriptors deviated from a normal distribution, necessitating non-parametric tests for further statistical analysis. We employed the Mann-Whitney U test to evaluate the statistical significance of differences between groups defined by semantic labels, ensuring the robustness of the feature selection process against non-normal distribution patterns.

### (2) Feature Importance Ranking

We used two machine learning models, logistic regression and random forests, to rank the descriptors in terms of their predictive power for semantic labels. This approach allowed us to identify linear and non-linear relationships between the descriptors and the labels, providing insights into the most important features.

For more information about our work, please refer to the following paper:

BiSAID: Bipolar Semantic Adjectives Icons and Earcons Dataset





