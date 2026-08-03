# A Comparative Federated Deep Learning Approach for Multi-Class Diabetic Retinopathy Detection

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-D00000?logo=keras)
![Federated Learning](https://img.shields.io/badge/Federated-Learning-success)

A privacy-preserving Deep Learning framework for **Multi-Class Diabetic Retinopathy (DR) Detection** using **Federated Learning (FL)**. The proposed framework enables multiple healthcare institutions to collaboratively train a shared diagnostic model without exchanging sensitive patient data.

---

## Overview

Traditional deep learning models rely on centralized medical datasets, creating privacy and regulatory challenges. This project implements a **Federated Learning** framework using the **Federated Averaging (FedAvg)** algorithm, allowing distributed model training while keeping patient data local to each participating institution.

A comparative evaluation was performed using four deep learning architectures:

- Custom CNN
- MobileNetV2
- VGG16
- ResNet50

---

## Project Architecture

The overall workflow consists of:

1. Image preprocessing using Gaussian filtering
2. Distribution of retinal fundus images across simulated healthcare institutions
3. Local model training on each client
4. Federated model aggregation using **FedAvg**
5. Global model evaluation on multi-class Diabetic Retinopathy classification

> **Note:** The workflow diagram from the conference paper can be added here.

```text
docs/
└── architecture.png
```

After adding the image, include:

```md
<p align="center">
  <img src="docs/architecture.png" alt="Federated Learning Workflow" width="850"/>
</p>
```

---

## Tech Stack

- Python
- TensorFlow / Keras
- Federated Learning (FedAvg)
- OpenCV
- NumPy
- Pandas
- Google Colab

---

## Experimental Results

| Model | Accuracy |
|-------|---------:|
| Custom CNN | 32% |
| MobileNetV2 | 76% |
| VGG16 | 73% |
| **ResNet50** | **78%** |

### Key Findings

- ResNet50 achieved the highest diagnostic accuracy (78%).
- MobileNetV2 provided competitive performance with lower computational cost, making it suitable for edge deployment.
- Federated Learning enabled collaborative model training while preserving patient privacy.

---

## Repository Structure

```text
.
├── notebooks/
├── reports/
├── paper/
└── README.md
```

- **notebooks/** – Jupyter notebooks containing model implementation and experiments.
- **reports/** – Project report, presentation, and supporting documentation.
- **paper/** – Conference paper and related resources.

---

## Conference Publication

This work resulted in the conference paper:

**A Federated Deep Learning Approach for Multi-Class Diabetic Retinopathy Detection.** :contentReference[oaicite:0]{index=0}

---

## Future Work

- Personalized Federated Learning
- Differential Privacy
- Secure Aggregation
- Communication-efficient optimization
- Large-scale multi-institution deployment

---

## Authors

- Regalagadda Mohith Varun
- Sreeram Reddy Nandem
- Gowthami Reddy Reddem
- Manoj Kumar Settipalli
- Dr. Satya Krishna Nunna
