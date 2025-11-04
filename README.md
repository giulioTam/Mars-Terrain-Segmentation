# 🪐 Mars Terrain Segmentation — ANN & Deep Learning Homework 2

This project was developed as part of the **Artificial Neural Networks and Deep Learning** course (A.Y. 2024–2025) at Politecnico di Milano.  
It focuses on building a **semantic segmentation** model to classify each pixel of grayscale Mars terrain images into one of five terrain classes.

---

## 📘 Overview
The task consists of predicting pixel-level class labels for 64×128 grayscale images of the Martian surface.  
Each pixel belongs to one of **five terrain categories**, while the background class (label `0`) is **ignored during evaluation**.

The project follows the structure of a Kaggle-style competition organized by the course instructors.

---

## ⚙️ Problem Description
- **Task:** Semantic segmentation  
- **Input:** Grayscale images (64×128 pixels)  
- **Output:** Predicted segmentation masks with pixel-level class labels  
- **Classes:** 5 terrain types (background excluded from evaluation)  
- **Metric:** Mean Intersection over Union (mIoU)  \[
\text{mIoU} = \frac{1}{|C|} \sum_{c \in C} \frac{TP_c}{TP_c + FP_c + FN_c}
\]
where \( C \) is the set of valid classes (excluding the background).

Leaderboard and final results were computed on hidden test subsets.


---

## 🚫 Restrictions
As required by the competition rules:
- **No pretrained models are allowed** — all neural networks must be trained **from scratch**.
- The use of pretrained backbones (e.g., ResNet, VGG, EfficientNet) is strictly forbidden.
- Models must be fully implemented and trained within the provided notebooks.

---

## 🧠 Model Development
The notebook includes:
- **Data preprocessing:** normalization, augmentation, and dataset split  
- **Model architecture:** convolutional neural network (CNN) built from scratch  
- **Loss function:** Cross-Entropy Loss  
- **Optimizer:** Adam  
- **Evaluation metric:** Mean IoU (ignoring class 0)  
- **Training strategy:** early stopping and learning rate scheduling  
- **Results:** training/validation curves and final performance on the test set  

---

## 🧪 Evaluation
Performance was assessed using **Mean Intersection over Union (mIoU)**:
\[
\text{mIoU} = \frac{1}{|C|} \sum_{c \in C} \frac{TP_c}{TP_c + FP_c + FN_c}
\]
where \( C \) is the set of valid classes (excluding the background).

Leaderboard and final results were computed on hidden test subsets.

---


## 👨‍💻 Authors
**Team [Your Team Name]**  
Artificial Neural Networks and Deep Learning — Politecnico di Milano  
A.Y. 2024–2025

---


## 📁 Repository Structure
