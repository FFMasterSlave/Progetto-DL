# Contrastive Machine Unlearning with Hyperbolic Embeddings

## Introduction
This project explores contrastive machine unlearning by applying contrastive learning techniques in both Euclidean and hyperbolic spaces. The aim is to unlearn specific data points or classes effectively while maintaining high model accuracy on retained data. 
I used CIFAR-10 and SVHN datasets to benchmark performance across unlearning scenarios and compare hyperbolic embeddings with standard Euclidean ones.

The approach is inspired by the article *"A Contrastive Approach to Machine Unlearning"* and introduces hyperbolic embeddings to evaluate the benefits of non-Euclidean geometry in unlearning tasks. The project includes:

Two main pipelines for single-class and random-sample unlearning.
ResNet architectures customized for Euclidean and hyperbolic embeddings, using libraries like Geoopt and Hypll for hyperbolic transformations.
Visualization tools to examine feature embeddings, retraining, and unlearning progress, with 3D t-SNE and convex hulls for better interpretability.

## Usage
All the code is inside the *contrastive_unlearning_project.ipynb*, so please refer to that. It's a Jupyter notebook with all the steps and more informations about the implementation.
Inside the other directories you'll find some images represenatative of the results of the pipeline in the various scenarios.

**ATTENTION**: as said in both the report and the notebook, the image results are just from a run because the unlearning algorithm is not deterministic.
This means that if you run the notebook, you can get lucky and see good results or be unlucky and find some cheap outcomes. 

## Installation
You'll fine all the necessary libraries inside a cell on the notebook.

**BE CAREFUL**: it is suggested to run the notebook on GPU, **however**, if you do it **MAKE SURE** you have the correct installation of CUDA toolkit. My version was the 11.8.
I didn't include it inside the notebook cause it has the potential of breaking everything.


