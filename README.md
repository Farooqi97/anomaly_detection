# Detecting Behavioral Anomalies – A Journey into Unsupervised ML

## 🧭 Overview

This repository is part of my learning journey into how anomalies behave in real-world scenarios — such as fraud, unusual performance in tests, or unexpected behavioral shifts. I wanted to understand not only *what* anomaly detection is, but *how* specific algorithms work and *why* some are better suited than others.

This project focuses on **Unsupervised Anomaly Detection** using three powerful algorithms:
- **Isolation Forest** (Tree-based, widely used in fraud/behavior shift)
- **Local Outlier Factor (LOF)** (Density-based, local anomaly detection)
- **Autoencoder** (Deep Learning-based)

It also explores how **AutoML** can simplify this process for non-experts.

---

## 🎯 What is Anomaly Detection?

Anomalies, or outliers, are data points that behave differently than the majority. In real-world systems, anomalies may indicate:
- 🔐 **Fraudulent transactions**
- ⚙️ **Machine failure or sensor error**
- 🧪 **A test sample behaving differently**
- 👤 **User behavior deviation**

---

## 🔍 Supervised vs Unsupervised Learning

| Learning Type      | What It Uses | Example                |
|--------------------|-------------|------------------------|
| **Supervised**     | Labeled data (Normal/Anomaly labels) | Credit card fraud with known cases |
| **Unsupervised**   | No labels (Model finds anomalies) | Unknown behavioral shifts in tests |

**Why Unsupervised for This Project?**  
In most anomaly problems (like fraud or rare test deviation), labeled anomalies are **rare or unknown**, so the model must discover them without being told.

---

## 🧪 Why I Chose These 3 Algorithms

From research and AI assistant guidance, these three algorithms represent different anomaly detection philosophies:

| Algorithm        | Why Chosen | Best Use Case |
|------------------|------------|---------------|
| **Isolation Forest** | Isolates anomalies by splitting data. Fast & interpretable. | Fraud, transaction anomalies |
| **LOF (Local Outlier Factor)** | Compares local density of a point to neighbors | Local behavior changes |
| **Autoencoder** | Learns to reconstruct data, large reconstruction error = anomaly | Complex behavioral patterns |

These three give a *complete view* — from statistical distance to deep learning complexity.

---

## 🧭 Flow of Understanding

### 🧠 Learning Path

Machine Learning
├── Supervised Learning
│   └── Needs labeled anomalies (not practical here)
└── Unsupervised Learning
    └── Anomaly Detection
        ├── Isolation Forest (Tree-based)
        ├── Local Outlier Factor (Density-based)
        └── Autoencoder (Neural network-based)
             ↓
          AutoML
          └── Automates model selection & tuning

## 🧪 Real-World Example: Behavioral Change in Test Samples

Imagine you have **1000 test samples**, and only a **few behave differently**.  
You’re asked: _“Which tests performed abnormally?”_

But you don’t have labels — you don’t know which ones are odd.

> This is where **Unsupervised Anomaly Detection** steps in.  
> Algorithms like Isolation Forest will "isolate" those unusual tests.  
> LOF will compare each test’s density to its neighbors.  
> Autoencoder will try to reconstruct normal tests and fail on odd ones.

---

## 🤖 Enter AutoML – Why It Matters

Many beginners struggle with:

* Which algorithm to pick?  
* How to tune parameters?  
* How to evaluate anomalies?

**AutoML solves this by:**  
✅ Automatically selecting the best anomaly algorithm  
✅ Tuning hyperparameters  
✅ Reducing manual trial-and-error

While this project first explores core concepts manually, **AutoML can turn this into a scalable pipeline** — especially useful in fraud detection systems or monitoring platforms.

---

## 🌱 Motivation

I started this project to understand **how anomalies behave in the real world**, beyond theory. My goal is to build an intuition:

* Why do anomalies occur?  
* How do algorithms detect them differently?  
* Can machines detect what humans miss?

This repository is my learning journey — shared openly for anyone exploring the same path.

---

## 🚀 Next Steps

* 🔍 Add simple code snippets (Isolation Forest, LOF, Autoencoder)  
* 🧪 Add synthetic test data experiment  
* 🤖 Integrate AutoML (PyCaret / H2O)

---

### 🏷️ Tags

`#MachineLearning` `#AnomalyDetection` `#IsolationForest` `#AutoML` `#UnsupervisedLearning`