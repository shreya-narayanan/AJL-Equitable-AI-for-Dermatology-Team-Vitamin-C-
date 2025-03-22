# Equitable AI for Dermatology: Team Vitamin C
---
## Project Description

This project was developed as part of the Spring 2025 Break Through Tech AI Studio, in collaboration with the Algorithmic Justice League (AJL). The initiative brings together AI Fellows from various universities to work on a real-world machine learning challenge hosted on Kaggle.

The goal of this challenge is to build a machine learning model that can classify 21 different dermatological conditions across diverse skin tones, using a subset of the Fitzpatrick17k dataset. The challenge addresses a pressing problem in dermatology AI: many existing models underperform on darker skin tones due to racially biased and non-inclusive training data.

AI is increasingly used in healthcare, including dermatology. However, when models are trained primarily on light skin, they often fail to generalize to people with darker skin tones mwhich often results in misdiagnoses, delayed treatment, and health disparities.

This project contributes to the broader real-world mission of algorithmic fairness by:

- Highlighting how data representation affects model performance.
- Evaluating and addressing bias using skin tone (Fitzpatrick Scale)
  
Our work aligns with AJL’s mission to reduce bias in AI and push for more equitable AI systems in healthcare.

---
## Team Members
- Mohani Adem
- April Guo-Yue
- [Melody He](https://github.com/melodyhe21)
- Madeleine Miller
- Shreya Narayanan

---
## Data Description

We used the dataset provided through the Kaggle competition, which is a curated subset of the Fitzpatrick17k dataset. It includes around 4,500 dermatology images across 21 skin conditions and a range of skin tones based on the Fitzpatrick Scale (1–6).

Some of the features inclue:
- label (target diagnosis),
- fitzpatrick_scale (self-reported skin tone),
- fitzpatrick_centaur (skin tone labeled by medical professionals),
- nine_partition_label and three_partition_label (diagnostic categories),

We did not use any external datasets, but we applied preprocessing and augmentation techniques to reduce class imbalance and improve model performance.

---
## Table of Contents
1. [Repository Structure](#repository-structure)
2. [Python Environment Set-up](#python-environment-set-up)
3. [Package Installation](#package-installation)
4. [Description](#description)
7. [Data](#data)
---
