# Contrastive Machine Unlearning with Hyperbolic Embeddings

## Introduction
This project explores contrastive machine unlearning by applying contrastive learning techniques in both Euclidean and hyperbolic spaces. The aim is to unlearn specific data points or classes effectively while maintaining high model accuracy on retained data. We use CIFAR-10 and SVHN datasets to benchmark performance across unlearning scenarios and compare hyperbolic embeddings with standard Euclidean ones.

The approach is inspired by the article "A Contrastive Approach to Machine Unlearning" and introduces hyperbolic embeddings to evaluate the benefits of non-Euclidean geometry in unlearning tasks. The project includes:

Two main pipelines for single-class and random-sample unlearning.
ResNet architectures customized for Euclidean and hyperbolic embeddings, using libraries like Geoopt and Hypll for hyperbolic transformations.
Visualization tools to examine feature embeddings, retraining, and unlearning progress, with 3D t-SNE and convex hulls for better interpretability.

