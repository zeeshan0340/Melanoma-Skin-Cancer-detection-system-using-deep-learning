# Melanoma Skin Cancer Detection Using Deep Learning

A deep learning-based computer vision system for automated melanoma skin lesion classification using dermoscopic images. The project explores and compares multiple convolutional neural network architectures, including a custom CNN and several pretrained transfer-learning models, to investigate their effectiveness for skin cancer image classification.

## Overview

Melanoma is one of the most serious forms of skin cancer, and early detection plays an important role in improving patient outcomes. However, accurate diagnosis from skin lesion images can be challenging and typically requires substantial clinical expertise.

This project investigates the use of deep learning and computer vision for automated melanoma detection. Multiple neural network architectures were trained and evaluated on a skin lesion image dataset to compare their classification performance.

The project follows an end-to-end deep learning workflow:

**Dataset → Preprocessing → Model Development → Transfer Learning → Training → Validation → Comparative Evaluation → Prediction**

The primary objective was to gain practical experience in developing deep learning models for medical image classification while investigating how different CNN architectures perform on the same medical imaging task.

---

## Objectives

The main objectives of this project were to:

* Develop an automated melanoma skin cancer classification system.
* Apply deep learning to medical image analysis.
* Preprocess and prepare skin lesion images for model training.
* Develop a custom CNN architecture as a baseline.
* Evaluate multiple pretrained CNN architectures using transfer learning.
* Compare the performance of different architectures.
* Identify an effective deep learning approach for melanoma classification.
* Gain practical experience in applying computer vision techniques to medical imaging.

---

## Dataset

The project used a skin lesion image dataset containing approximately **13,000 images**.

The dataset was organized into training and testing subsets:

| Split     |     Images |
| --------- | ---------: |
| Training  |     10,682 |
| Testing   |      3,561 |
| **Total** | **14,243** |

> **Note:** The image counts above reflect the dataset split recorded during the project. The original dataset size was also referred to as approximately 13,000 images during development; therefore, the exact dataset provenance and split should be verified against the final repository before publication.

The images represent skin lesions that are used for classification of melanoma-related cases.

### Dataset Considerations

Medical imaging datasets can contain challenges such as:

* Variations in image quality
* Different lesion sizes and appearances
* Illumination and color differences
* Class imbalance
* Similar visual characteristics between benign and malignant lesions

These factors make preprocessing and model evaluation particularly important in medical AI applications.

---

## Deep Learning Models

To investigate the effect of different architectures, several CNN-based models were implemented and evaluated.

### Custom CNN

A custom convolutional neural network was developed as a baseline model for the classification task.

The model follows the conventional CNN pipeline of:

**Convolution → Activation → Pooling → Feature Extraction → Classification**

This provided a baseline against which pretrained architectures could be compared.

### Transfer Learning Models

The project also experimented with several established CNN architectures:

* **ResNet50**
* **ResNet101**
* **DenseNet121**
* **MobileNetV2**
* **VGG16**
* **VGG19**
* **InceptionV3**

Transfer learning was used to leverage representations learned from large-scale image datasets and adapt them to the skin lesion classification problem.

---

## Model Training

The models were trained using deep learning frameworks including:

* Python
* TensorFlow
* Keras

The general training pipeline consisted of:

1. Loading the skin lesion dataset.
2. Preparing training and testing images.
3. Applying image preprocessing.
4. Preparing images for CNN input.
5. Building the classification models.
6. Training the models on the training dataset.
7. Monitoring validation performance.
8. Evaluating trained models.
9. Comparing model performance.

---

## Experimental Results

One of the experiments achieved the following validation performance:

| Metric              |     Result |
| ------------------- | ---------: |
| Validation Accuracy | **91.34%** |
| Validation Loss     |  **0.232** |

These results demonstrate the potential of deep learning models for automated skin lesion classification.

However, accuracy alone is not sufficient to establish clinical effectiveness. For a medical AI system, additional metrics such as **precision, recall, F1-score, sensitivity, specificity, ROC-AUC, and confusion matrices** should be considered.

---

## Comparative Model Evaluation

A major component of the project was the comparison of different CNN architectures.

The comparison included:

| Model       | Approach                     |
| ----------- | ---------------------------- |
| Custom CNN  | Baseline deep learning model |
| ResNet50    | Transfer learning            |
| ResNet101   | Transfer learning            |
| DenseNet121 | Transfer learning            |
| MobileNetV2 | Transfer learning            |
| VGG16       | Transfer learning            |
| VGG19       | Transfer learning            |
| InceptionV3 | Transfer learning            |

This comparative approach provides insight into how different feature extraction architectures behave when applied to the same medical image classification problem.

---

## Technologies Used

### Programming & Frameworks

* Python
* TensorFlow
* Keras

### Deep Learning

* Convolutional Neural Networks
* Transfer Learning
* Image Classification
* Feature Extraction

### Computer Vision

* Medical Image Analysis
* Image Preprocessing
* Skin Lesion Classification

### Development Environment

* Google Colab
* Jupyter Notebook
* Kaggle Dataset/API

---


## Research Workflow

The project was developed as an end-to-end medical AI experiment rather than simply training a single classification model.

### 1. Dataset Preparation

The skin lesion images were collected and organized for deep learning experiments.

### 2. Image Preprocessing

Images were prepared into a format suitable for CNN-based models.

### 3. Baseline Development

A custom CNN was developed to establish a baseline classification performance.

### 4. Transfer Learning

Several established CNN architectures were investigated to determine whether pretrained feature representations could improve classification.

### 5. Model Training

Each architecture was trained and evaluated using the same general classification task.

### 6. Comparative Analysis

The models were compared to understand the strengths and weaknesses of different architectures.

### 7. Performance Evaluation

Validation performance was analyzed using classification metrics and model training behavior.

---

## Why Multiple Architectures?

Different CNN architectures learn visual representations in different ways.

**ResNet** uses residual connections that enable the training of deeper networks.

**DenseNet** promotes feature reuse through dense connectivity between layers.

**MobileNetV2** is designed for computational efficiency and lightweight deployment.

**VGG** provides a relatively simple and well-established deep CNN architecture.

**InceptionV3** uses multi-scale feature extraction through its Inception modules.

Comparing these architectures provides a broader understanding of their suitability for medical image classification rather than relying on a single model.

---

## Key Learning Outcomes

Through this project, I gained practical experience in:

* Medical image classification
* Deep learning model development
* CNN architecture design
* Transfer learning
* TensorFlow and Keras
* Dataset preparation
* Image preprocessing
* Model training
* Validation and evaluation
* Comparative experimentation
* Interpreting deep learning results

The project also strengthened my interest in **Medical AI, Computer Vision, and Deep Learning**, particularly in the development of reliable AI systems for healthcare applications.

---

## Limitations

This project is primarily an experimental and academic deep learning system and should **not be considered a clinical diagnostic tool**.

Important limitations include:

* Model performance depends strongly on the quality and representativeness of the dataset.
* Dataset bias may affect generalization to different patient populations and imaging environments.
* A high classification accuracy does not necessarily imply clinical reliability.
* Additional external validation would be required before considering real-world clinical deployment.
* More comprehensive evaluation using sensitivity, specificity, F1-score, ROC-AUC, calibration, and external test datasets would strengthen the study.

---

## Future Work

Future improvements could focus on developing a more robust and clinically relevant medical AI system.

Potential research directions include:

* Evaluation on independent external datasets
* Addressing class imbalance
* Data augmentation and advanced preprocessing
* Hyperparameter optimization
* Explainable AI for medical predictions
* Grad-CAM and attention-based visualization
* Vision Transformer architectures
* Ensemble learning
* Multimodal medical AI
* Lesion segmentation before classification
* Uncertainty estimation
* Model calibration
* Robustness testing across datasets
* Lightweight models for real-time deployment

A particularly interesting direction is combining **computer vision with multimodal learning and medical language models** to move from simple image classification toward more interpretable and clinically useful medical AI systems.

---

## Disclaimer

This project is intended for **educational and research purposes only**. It is not a medical device and should not be used to diagnose melanoma or make clinical decisions. Any real-world medical application would require extensive clinical validation, regulatory approval, and evaluation by qualified medical professionals.

---

## Author

**Zeeshan Hassan**

BS Computer Science
Research Interests: **Deep Learning, Computer Vision, Medical AI, Multimodal Learning, Large Language Models, and Retrieval-Augmented Generation (RAG)**

---

## License

This project is intended for academic and research purposes. Please add an appropriate open-source license to the repository if you intend to permit reuse or modification.

```
© 2026 Zeeshan Hassan
```
