# 🧠 Deep Learning-Based Depression Detection from Brain MRI

An AI-assisted multimodal deep learning framework for detecting **Major Depressive Disorder (MDD)** using **3D structural brain MRI scans** and **clinical metadata**.

Developed as a Graduation Project at **King Khalid University – Department of Computer Science**.

---

# 📌 Overview

This project presents an end-to-end deep learning pipeline for depression detection from **T1-weighted 3D brain MRI** data. The system combines:

- 3D MRI anatomical features
- Clinical metadata:
  - Age
  - Sex
  - Education
  - HAMD score

The framework uses a **multimodal late-fusion architecture** consisting of:

- 3D CNN imaging branch
- Squeeze-and-Excitation (SE) attention
- Clinical metadata MLP branch
- Binary classification head

The system classifies subjects into:
- Healthy Control (HC)
- Major Depressive Disorder (MDD)

---

# 👨‍💻 Project Team

- Fahad Al Nahi
- Ibrahim Hurubi
- Fahad Al-Mubarak
- Abdullah Alshaharani
- Ali Muyini

### Supervisor
Dr. Mohamed Ghouse

---

# 🚀 Features

✅ 3D MRI volumetric analysis  
✅ Multimodal learning (MRI + clinical metadata)  
✅ 3D CNN + SE Attention architecture  
✅ Healthy-brain autoencoder pretraining  
✅ Medical-grade MRI preprocessing  
✅ Grad-CAM explainability support  
✅ FastAPI backend API  
✅ Next.js frontend prototype  
✅ Independent test-set evaluation  

---

# 🏗️ System Architecture

## MRI Imaging Branch
- 3D Convolutional Neural Network
- Learns anatomical brain features
- Preserves volumetric spatial information

## Clinical Metadata Branch
Processes:
- Sex
- Age
- Education
- HAMD score

Using:
- Multi-Layer Perceptron (MLP)

## Fusion Layer
Combines MRI and clinical representations for binary classification.

---

# 📂 Project Structure

```bash
├── notebook.ipynb
├── best_multimodal_model.pth
├── blueprint.pth
├── train_multimodal.csv
├── val_multimodal.csv
├── test_multimodal.csv
├── healthy_train_only.csv
├── frontend/
│   ├── Next.js
│   ├── React
│   └── Tailwind CSS
├── backend/
│   ├── FastAPI
│   └── main.py
└── README.md
```

---

# 📊 Dataset

The project uses large-scale public neuroimaging datasets for Major Depressive Disorder (MDD) research.

## Datasets
- DIRECT Phase II Dataset
- REST-meta-MDD Dataset

## Imaging Type
- T1-weighted Structural MRI (sMRI)

## Clinical Features
- Sex
- Age
- Education
- HAMD score

## Dataset Split

| Split | Samples |
|---|---|
| Training | 1732 |
| Validation | 217 |
| Test | 217 |
| Healthy-only Pretraining | 736 |

---

# ⚙️ Technologies Used

## AI / Deep Learning
- Python
- PyTorch
- NumPy
- Pandas
- Scikit-learn

## Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS

## Backend
- FastAPI
- Uvicorn
- ngrok

## Development Tools
- Google Colab
- GitHub

---

# 🔬 Training Pipeline

## Phase 1 — Multimodal Data Engineering
- MRI-clinical data fusion
- Z-score normalization
- Stratified dataset splitting

## Phase 2 — Medical-Grade Dataset Engine
- Dynamic brain cropping
- MRI resizing (64×64×64)
- 3D augmentations:
  - Cutout
  - Gaussian noise
  - Gamma adjustment
  - Z-axis flipping

## Phase 3 — Healthy Brain Autoencoder
- Trained only on Healthy Controls
- Learns normative anatomical representation

## Phase 4 — Multimodal Classification
- 3D CNN + Clinical MLP
- Late fusion architecture
- Binary classification

---

# 📈 Model Performance

| Metric | Score |
|---|---|
| Accuracy | 97% |
| AUC | 0.9870 |
| Sensitivity | 0.9440 |
| Specificity | 1.0000 |

---

# 🖥️ Web Prototype

The system includes a web-based interface that allows users to:

1. Upload/select MRI scans
2. Enter clinical metadata
3. Run AI analysis
4. View prediction results
5. Display confidence score
6. Visualize Grad-CAM heatmaps

---

# 🔍 Explainability

The framework supports **Grad-CAM-style visualization** to highlight anatomical regions contributing to predictions, improving interpretability and clinical trust.

---

# ⚠️ Disclaimer

This project is an academic research prototype intended for educational and research purposes only.

It is **not** a certified clinical diagnostic system.

---

# 📚 Documentation

Project chapters include:

- Chapter 1 — Introduction
- Chapter 2 — Literature Review
- Chapter 3 — Methodology and Analysis
- Chapter 4 — System Design
- Chapter 5 — System Implementation
- Chapter 6 — Model Development
- Chapter 7 — System Testing
- Chapter 8 — Future Work and Conclusion

---

# 🔗 Repository

GitHub Repository:
https://github.com/Ibrahim-Hurubi/mri-depression-detection
