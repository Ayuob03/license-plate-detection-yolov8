# 🚗 License Plate Detection Using YOLOv8

This repository contains a complete pipeline for **detecting license plates in images and video** using **YOLOv8**, trained on a global license plate dataset from Roboflow.

The goal is to:
- Detect license plates in road scenes 📦
- Use the detections later for OCR and tracking (extension of this project) 🔍

---

## 📦 Dataset

The model is trained on a **global license plate detection dataset** from Roboflow Universe:

- One main class: `license_plate`
- Mixed countries and plate styles
- Exported in **YOLOv8 format** (train / valid / test + `data.yaml`)

The dataset is downloaded in Colab using the Roboflow API.

---

## 🧠 Model

We use:

- **YOLOv8n (nano)** as a base model, pretrained on COCO  
- Then fine-tune it on the license plate dataset

Frameworks:

- `ultralytics` (YOLOv8)
- `roboflow` (dataset management)
- `opencv-python`
- `easyocr` (for future OCR extension)

---

## 🚀 Training (Colab)

Install dependencies:

```python
!pip install ultralytics roboflow
