# 🖼️ Image Captioning – Fine-tuning & Inference

This project focuses on **Image Captioning**, generating natural language descriptions for images using a deep learning model. It supports **fine-tuning on custom datasets** and running inference using pre-trained checkpoints.

---

## 📌 Project Overview

Image Captioning is a multi-modal task that combines:
- **Computer Vision** (image feature extraction)
- **Natural Language Processing** (caption generation)

In this project, a pre-trained image captioning model is provided and can be **fine-tuned on a new dataset** to improve performance for specific domains.

---

## 📂 Resources

- **Pre-trained Checkpoint**  
  Download here:  
  https://drive.google.com/file/d/1A1yZY8yMIED6cXU731xGKxA9Jr8a9BNk/view?usp=drive_link

- **Tokenizer / Vocabulary (Pickle File)**  
  Download here:  
  https://drive.google.com/file/d/10PydPz1ZIXKr9xzD5r_eEqFESZpr6L8C/view?usp=drive_link

- **Testing & Demo Notebook (Google Colab)**  
  https://colab.research.google.com/drive/1i8_RCvPSJnteqtBjIACkF42C1AJfRQFN

---

## 🧠 Model Architecture (High-level)

- **Image Encoder**: CNN-based feature extractor (e.g. ResNet or similar backbone)
- **Text Decoder**: Sequence model (LSTM / GRU / Transformer)
- **Tokenizer**: Pre-built vocabulary loaded from pickle file
- **Loss Function**: Categorical Cross-Entropy
- **Optimizer**: Adam / AdamW

---

## 🔧 Fine-tuning Guide

### 1️⃣ Dataset Preparation

Your dataset should include:
- Images (JPEG / PNG)
- Captions (one or multiple captions per image)

Recommended structure:
