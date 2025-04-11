# Equitable AI for Dermatology: Team Vitamin C
---
## Team Members
- Mohani Adem | @mohaniadem | Performed data augmentation and preprocessing
- April Guo-Yue 
- Melody He | @melodyhe21 | Built EfficientNet CNN Model and fine tuned
- Madeleine Miller | Built ResNet CNN Model and fine tuned
- Shreya Narayanan | @shreya-narayanan | Built InceptionV3 Model and fine tuned
---
## Table of Contents
1. [Project Highlights](#project-highlights)
2. [Environment Set-up](#environment-set-up)
3. [Project Overview](#project-overview)
4. [Data Description](#data-description)
5. [Data Exploration](#data-exploration)
6. [Model Development](#model-development)
7. [Next Steps](#next-steps)

## Project Highlights
- Developed deep learning models to classify **21 dermatological conditions** from images across a diverse range of skin tones.
- Tackled racial bias in dermatology datasets using inclusive modeling and preprocessing.
- Evaluated and compared three CNN models: **EfficientNet**, **ResNet**, and **InceptionV3**.
- Addressed underrepresentation of darker skin tones through augmentation and model fine-tuning.
- Aligned with the mission of the Algorithmic Justice League to build equitable AI systems in healthcare.

## Set-up & Execution

### Environment
- Python 3.8+  
- Jupyter Notebook or Google Colab  
- Libraries: TensorFlow, Keras, NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn  

### To Run the Project
1. Clone the repository  
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
3. Open and run the following notebooks:
efficient_net_model.ipynb  
inceptionv3.ipynb  
updated_inceptionv3.ipynb  

## Project Overview

This project was developed as part of the Spring 2025 Break Through Tech AI Studio, in collaboration with the Algorithmic Justice League (AJL). The initiative brings together AI Fellows from various universities to work on a real-world machine learning challenge hosted on Kaggle.

The goal of this challenge is to build a machine learning model that can classify 21 different dermatological conditions across diverse skin tones, using a subset of the Fitzpatrick17k dataset. The challenge addresses a pressing problem in dermatology AI: many existing models underperform on darker skin tones due to racially biased and non-inclusive training data.

AI is increasingly used in healthcare, including dermatology. However, when models are trained primarily on light skin, they often fail to generalize to people with darker skin tones mwhich often results in misdiagnoses, delayed treatment, and health disparities.

This project contributes to the broader real-world mission of algorithmic fairness by:

- Highlighting how data representation affects model performance.
- Evaluating and addressing bias using skin tone (Fitzpatrick Scale)
  
Our work aligns with AJL’s mission to reduce bias in AI and push for more equitable AI systems in healthcare.

---
## Data Description & Exploration

We used the dataset provided through the Kaggle competition, which is a curated subset of the Fitzpatrick17k dataset. It includes around 4,500 dermatology images across 21 skin conditions and a range of skin tones based on the Fitzpatrick Scale (1–6).

Some of the features inclue:
- label (target diagnosis),
- fitzpatrick_scale (self-reported skin tone),
- fitzpatrick_centaur (skin tone labeled by medical professionals),
- nine_partition_label and three_partition_label (diagnostic categories),

We did not use any external datasets, but we applied preprocessing and augmentation techniques to reduce class imbalance and improve model performance.

---

## Model Development

We implemented and fine-tuned three different Convolutional Neural Network architectures:

### EfficientNet (by Melody He)
- Lightweight and scalable  
- Achieved strong accuracy with fewer parameters  
- Fine-tuned using learning rate decay and dropout  

### ResNet (by Madeleine Miller)
- Deep residual connections improved feature learning  
- Resistant to vanishing gradient problem  
- Performed well on complex diagnostic features  

### InceptionV3 (by Shreya Narayanan)
- Multi-scale feature extraction  
- Fine-tuned for deeper layer activation  
- Tuned with dropout and image augmentation  

Each model was trained using stratified sampling to preserve diversity across skin tones.

---

## Results & Key Findings

| Model        | Observations                                                       |
|--------------|--------------------------------------------------------------------|
| EfficientNet | High accuracy and generalizability across most skin tones          |
| ResNet       | Good baseline, robust but slightly less sensitive to darker tones  |
| InceptionV3  | Improved performance on underrepresented tones with augmentation   |

### Key Takeaways
- Augmentation improved model robustness on darker skin tones  
- There’s a consistent performance gap between light and dark skin tones  
- No single model was universally best — performance varied by skin tone category  
- Bias persists even after preprocessing, highlighting the need for diverse datasets

---

## Impact Narrative

AI in healthcare must be **inclusive** to avoid perpetuating disparities.

Our work directly addresses this challenge in dermatology by:
- Identifying performance differences across Fitzpatrick skin tones  
- Demonstrating how architectural choices and preprocessing impact fairness  
- Building models that begin to close the gap in diagnostic performance on darker skin  

We hope this project contributes toward building **equitable AI systems** that serve **all communities**, not just those historically overrepresented in training data.

---

## Next Steps & Future Improvements

- Integrate **fairness metrics** such as *Equalized Odds* and *Disparate Impact*  
- Use **Grad-CAM** for model interpretability and to highlight decision areas  
- Incorporate **additional diverse datasets** to expand generalization  
- Work with **dermatologists and domain experts** for validation and feedback  
- Explore **bias mitigation techniques** such as reweighting or adversarial training  
