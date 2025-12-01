
# 14 Student Distillation for high-end compute-intensive DL process to run on low-end GPU

## Overview

This project showcases the efficacy of **Knowledge Distillation (KD)** across three core computer vision tasks: **Image Classification**, **Semantic Segmentation (Edge Detection)**, and **Image Restoration (Super-Resolution)**.

The primary goal is to demonstrate that lightweight **Student Models** can inherit the high performance of heavy **Teacher Models**, achieving significant **model compression** and **faster inference speed** for real-world deployment.

---

## About the Authors (Group 5) 

| Name | Roll Number | Department |
| :--- | :--- | :--- |
| **Suryaa Thirumurugan** | EE23B077 | Electrical Engineering |
| **Shree Hari MG** | ME23B201 | Mechanical Engineering |

---

##  Execution Procedure: Getting Started

All three tasks are designed to be executed sequentially in the **Google Colaboratory (Colab)** environment. 
All required datasets are downloaded through code during execution.

### Prerequisites
1. Ensure all `.ipynb` notebooks and `.pth` model files are uploaded.
2. All required libraries install automatically in each notebook.
3. Make sure file paths are in match with your environment
---

### 1. Semantic Segmentation (Edge Detection)

- File: `edge_detection.ipynb`
- Block 1 → Train & save models  
- Block 2 → Upload test image and run inference  
- Models saved to: `/content/saved_models/`

---

### 2. Image Classification

- Teacher: `resnet101.ipynb`
- Distillation: `student_resnet101_upgraded.ipynb` (Contains both Student model and tiny student model)
- final_result.ipynb - Contains results (time and accuracy)
- Test images: `test_images1/`
- Final model files:
  - `teacher_resnet101_best.pth`
  - `student_mobilenet_cifar_best.pth`
  - `student_mobilenet_0.5x_best.pth`
- NOTE: You will have to run the resnet101.ipynb to get the teacher weights file.

---

### 3. Image Restoration (Super-Resolution)

- File: `image_rest.ipynb`
- Runs automatically with random downloaded image

---

