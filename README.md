# VGG16 Framework for Multi-Class Image Classification

**Project Type:** Team Project  
**Institution:** King Abdullah II School of Information Technology – University of Jordan  

This project presents a deep learning framework for multi-class image classification based on the VGG16 convolutional neural network.

The work was conducted as a team-based academic project and resulted in a technical research paper titled:

**“Attention-Enhanced VGG16 with Transfer Learning for Multi-Class Image Classification”**

The framework addresses the challenge of classifying visually heterogeneous object categories using a controlled and systematic deep learning pipeline.

---

## Problem Overview

The task is formulated as a five-class image classification problem with the following categories:

- Car  
- Building  
- Person  
- Tree  
- Lab  

The dataset contains natural RGB images with high inter-class diversity in terms of:
- Shape  
- Texture  
- Scale  
- Illumination  
- Background complexity  

This diversity makes the classification task non-trivial, especially when training deep models on a moderately sized dataset.

---

## Methodology

The proposed framework is built on the VGG16 architecture and follows a structured experimental design:

- VGG16 backbone used as a feature extractor (`include_top=False`)
- Custom classification head:
  - Global Average Pooling  
  - Dropout  
  - Fully connected layer  
  - Softmax output for 5 classes  
- Models trained from scratch and under controlled settings  
- Fine-tuning strategy applied to higher convolutional layers  
- Training stabilization techniques:
  - Early stopping  
  - Learning rate scheduling  

The project systematically compares:

- Baseline VGG16 (trained from scratch)  
- Refined VGG16 with architectural improvements  
- Proposed VGG16 with training stabilization  
- Transfer learning using ImageNet-pretrained VGG16  

---

## Results

Key findings reported in the paper:

| Model              | Accuracy |
|--------------------|----------|
| Baseline VGG16     | 73%      |
| Refined VGG16      | 91%      |
| Proposed VGG16     | 93%      |
| Pretrained VGG16   | 99%      |

The proposed VGG16 model trained from scratch achieves **93% accuracy**, demonstrating that:

- Careful architectural refinement  
- Lightweight classification heads  
- Training stabilization strategies  

can significantly enhance the performance of classical CNN architectures without relying on pretrained weights.

---

## Repository Content

Only the core deep learning model notebook is included in this repository:

- `VGG16_.ipynb` – Implementation of the VGG16-based classification framework

Data preprocessing notebooks are intentionally excluded to keep the repository focused on:
- Model architecture  
- Training strategy  
- Deep learning methodology  

The complete workflow, experimental design, and evaluation details are documented in the accompanying research paper.

---

This project demonstrates:

- Practical deep learning experimentation  
- CNN architecture design  
- Controlled model comparison  
- Academic-level documentation and analysis  
- Team-based research and implementation
