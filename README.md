## Automated Defect Detection in TIG Welds

## 📌 Problem Definition
Efforts have been made in the past to address TIG welding defect classification using various 
techniques. Traditional approaches typically involved manual inspection, where human experts 
visually examined welds to identify and classify defects. However, this manual inspection 
process is time-consuming, subjective, and prone to errors.The purpose of this project is to find best model for TIG welding defect classification in steel. We aim to evaluate the performance and effectiveness of models in accurately identifying and classifying welding defects in real-time scenarios. <br>

## 🔗 Dataset:

<a href='https://www.kaggle.com/datasets/danielbacioiu/tig-stainless-steel-304' target="_blank"><img alt='Kaggle' src='https://img.shields.io/badge/Kaggle-100000?style=for-the-badge&logo=Kaggle&logoColor=20beff&labelColor=black&color=FFFFFF'/></a><br>

<img src = "weld_assets/Screenshot 2025-02-05 160049.png">

<br >
<img src = "weld_assets/Screenshot 2025-02-05 160103.png">
<br>

## 📓 Data Preprocessing and augmentation techniques 

➡️ Image Resizing: Steel TIG welding defect images (originally 1,280 × 700 pixels) were resized to 250 × 250 pixels to standardize dimensions and reduce computational complexity.

➡️ Normalization: Pixel values were normalized to a range of 0-1 by dividing by 255.0, ensuring consistency across images for better deep learning model convergence.

➡️ Grayscale to RGB Conversion: Since the original images were in grayscale, channel replication was applied to convert them into three-channel RGB format for improved model performance.

➡️ Enhancing Model Training: The transformation to RGB format allows deep learning models to leverage transfer learning architectures effectively, improving training robustness.

➡️ Preprocessing Impact: Standardization, normalization, and RGB conversion collectively optimized image inputs for deep learning analysis, ensuring uniformity and better feature extraction.

## 📓 Model Architecture

<img src = "weld_assets/Screenshot 2025-02-05 160212.png"><br>

By utilizing transfer learning, the models benefited from the learned representations of the base architectures, enhancing their ability to accurately classify welding defects.<br>

## 📓 Overview

| Transfer Learning Models Applied            | Accuracy |
| ----------------- | ------------------------------------------------------------------ |
| VGG16 | 96.83% |
| VGG19 | 94.17% |
| DenseNet169 | 98.27% |
| InseptionV3 | 97.71% |
<br>

## 👉 Application

Automatic welding defect detection offers several advantages over manual inspection methods such as Increased accuracy, Enhanced productivity, Consistency and reliability, Early detection and prevention, Safety improvement etc.
<br>

## 👉 Conclusion

Models such as VGG16, DenseNet169, and InceptionV3 demonstrated strong generalization 
capabilities and achieved higher accuracy in classifying steel defects

 
