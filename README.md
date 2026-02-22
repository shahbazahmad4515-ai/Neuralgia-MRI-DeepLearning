# Neuralgia-AI: Deep Learning for Trigeminal Neuralgia Detection

## 🏥 Project Overview
This project focuses on the automated detection of **Trigeminal Neuralgia** using 3D MRI (NIfTI) neuroimaging. Diagnosing this condition is challenging because it involves microscopic nerve-vessel compressions. This AI system automates the identification process using Convolutional Neural Networks (CNNs).

## 🚀 Key Technical Features
- **Data Pipeline:** Processed 3D NIfTI volumes from the OpenNeuro `ds005713` dataset.
- **Nerve-Focus Cropping:** Implemented a custom ROI (Region of Interest) crop to focus the AI on the brainstem and trigeminal nerve.
- **Model:** Leveraged **VGG16 Transfer Learning** with fine-tuning on a T4 GPU.
- **Handling Imbalance:** Optimized performance for a dataset with extreme subject imbalance (Healthy vs. Neuralgia) using class-weighting and probability thresholding.

## 📊 Performance Analysis
- **High Sensitivity (Recall):** The model prioritizes catching every neuralgia case, achieving a high recall rate essential for medical screening.
- **Architecture:** Balanced the trade-off between Precision and Recall to ensure clinical utility.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** TensorFlow, Keras, Nibabel, OpenCV, Scikit-learn
- **Platform:** Google Colab (T4 GPU)
