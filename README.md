# Adversarial Attacks on MNIST with TensorFlow & ART

A hands-on notebook demonstrating adversarial attacks on neural networks using the MNIST dataset and TensorFlow, powered by the Adversarial Robustness Toolbox (ART).

---

## Table of Contents

- [Project Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Model Architectures](#model-architectures)
- [Adversarial Attacks](#adversarial-attacks)
- [Defense Strategies](#defense-strategies)
- [Results & Insights](#results--insights)
- [Getting Started](#getting-started)
- [References](#references)

---

## Project Overview

This notebook explores the vulnerability of deep learning models to adversarial examples, using the MNIST digit classification task to demonstrate attack and defense techniques. The project compares the robustness of different architectures and attack methods using ART, highlighting the importance of adversarial robustness[attached_file:1].

---

## Tech Stack

- TensorFlow 2.x
- Keras
- numpy
- matplotlib
- Adversarial Robustness Toolbox (`art`)

---

## Dataset

- **MNIST**: Handwritten digit dataset. Loaded via Keras and numpy, with normalization and train/test split[attached_file:1].

---

## Model Architectures

- Fully connected neural network with one and multiple hidden layers
- Deep model with 5 dense layers (ReLU)
- CNN model with 2D convolution and pooling layers
- All benchmarks use accuracy on test data for comparison[attached_file:1]

---

## Adversarial Attacks

Implemented attacks:
- Fast Gradient Sign Method (FGSM)
- Carlini & Wagner (L2/Inf)
- Projected Gradient Descent (PGD/APGD)
- Momentum Iterative Method (MIM)

Attacks are generated and evaluated on trained models, comparing efficacy and visual examples[attached_file:1].

---

## Defense Strategies

- Adversarial training (with FGSM) to improve robustness
- Effect of defenses is measured against attacks and reported[attached_file:1]

---

## Results & Insights

- Adversarial attacks can dramatically reduce model test accuracy, even with small input perturbations.
- Robust architectures or adversarial training can recover some accuracy loss but remain vulnerable to stronger iterative attacks.
- Transferability of attacks and differences in norm constraints are evaluated and visualized[attached_file:1].

---

## Getting Started

### Requirements

