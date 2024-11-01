# Contrastive Machine Unlearning with Hyperbolic Embeddings

## Introduction
This project explores contrastive machine unlearning by applying contrastive learning techniques in both Euclidean and hyperbolic spaces. 

The aim is to unlearn specific data points or classes effectively while maintaining high model accuracy on retained data. 

The approach is inspired by the article *"A Contrastive Approach to Machine Unlearning"* and introduces hyperbolic embeddings to evaluate the benefits of non-Euclidean geometry in unlearning tasks. 

The project includes:

  - Two main pipelines for single-class and random-sample unlearning.
  - ResNet architectures customized for Euclidean and hyperbolic embeddings, using Hypll library for hyperbolic transformations.
  - Visualization tools to examine feature embeddings, retraining, and unlearning progress, with 3D t-SNE and convex hulls for better interpretability.

Folowing the original article, I used [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) and [SVHN](http://ufldl.stanford.edu/housenumbers/) datasets to benchmark performance across unlearning scenarios and compare hyperbolic embeddings with standard Euclidean ones.

## Usage
All the code for the project is inside the *contrastive_unlearning_project.ipynb*. 

It's a Jupyter notebook with detailed steps and more informations about the theory and implementation.

Inside the directory *experiments* you'll find some images represenatative of the results of the pipeline in the various scenarios.

## Installation
All the necessary libraries will be properly installed through the notebook except for the **torch** package and **Nvidia Cuda Toolkit**.

These packages are **essential**, so why i didn't include them?

Unfortunately, the Nvidia Cuda Toolkit is hardware dependent so you must install it on your own.

The whole project was done with the latest version of Pytorch for Cuda 11.8.
