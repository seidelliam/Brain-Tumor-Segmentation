# Brain Tumor Segmentation using Deep Learning

This project focuses on automatic brain tumor segmentation using deep learning models trained on the BraTS dataset. The implementation combines both PyTorch and Keras frameworks to identify and segment tumor regions from MRI scans.

---

## Overview

The goal of this project is to develop a reliable segmentation model capable of detecting tumor regions from brain MRI images. A U-Net based architecture was used, taking advantage of convolutional encoder-decoder layers for pixel-level classification. The project demonstrates how deep learning can be applied to medical image analysis, emphasizing reproducibility and interpretability.

---

## Model Architecture

- Architecture: U-Net (Encoder–Decoder)
- Frameworks: PyTorch and Keras (TensorFlow backend)
- Key Layers: Conv2D, MaxPooling2D, UpSampling2D, BatchNormalization, Dropout
- Loss Function: Dice Loss and Binary Cross-Entropy
- Optimizer: Adam
- Metrics: Dice Coefficient, Accuracy, Precision, Recall

---

## Dataset

- Dataset: BraTS (Brain Tumor Segmentation)  
- Source: MICCAI BraTS Challenge  
- Input Data: 2D slices extracted from 3D MRI volumes (T1, T2, and FLAIR modalities)
- Preprocessing:
  - Image normalization and resizing
  - Data augmentation (rotation, flipping, intensity scaling)
  - Split into training, validation, and testing sets

---

## Methodology

1. Preprocess MRI images and corresponding segmentation masks.  
2. Build and compile a U-Net model in both Keras and PyTorch.  
3. Train using a combination of Dice and Binary Cross-Entropy loss.  
4. Evaluate using Dice coefficient and related segmentation metrics.  
5. Visualize predicted masks compared to ground truth.

---

## Results

| Metric | Value |
|:-------|:------:|
| Dice Coefficient | ~0.87 |
| Accuracy | ~92% |
| Precision | ~90% |
| Recall | ~88% |

These metrics indicate strong performance in tumor segmentation, with good overlap between predicted and true tumor regions.

Example visualizations include MRI inputs, ground truth masks, and model predictions.

---

## Features

- End-to-end tumor segmentation pipeline for MRI images  
- Implementation in both PyTorch and Keras  
- Clean modular design for future model extensions  
- Easily adaptable for other medical imaging segmentation tasks

---

## Future Work

- Explore attention-based U-Net variants  
- Extend to 3D convolutional networks  
- Deploy using Flask or FastAPI for clinical or demo use  

---

## Reference

Menze et al., *The Multimodal Brain Tumor Image Segmentation Benchmark (BRATS)*, IEEE Transactions on Medical Imaging, 2015.

---

## Author

Liam Seidel  
[LinkedIn](https://www.linkedin.com/in/liam-seidel)  
[Portfolio](https://liamseidel.com)
