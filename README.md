# Vehicle License Plate Detection System

This project implements a license plate detection system using two deep learning approaches: **YOLOv11** and **Faster R-CNN**. The system is designed to detect vehicle license plates in various lighting conditions and orientations.

---

## 🚀 Features

- **Two model architectures:**
  - `YOLOv11` for fast inference
  - `Faster R-CNN` for high precision

- **Data augmentation techniques:**
  - Random horizontal flips
  - Rotation (−15° to 15°)
  - Brightness/contrast adjustments
  - Gaussian blur
  - Scaling (90–110%)
  - Translation (±10%)

- **OCR Integration**
  - Uses Tesseract for license plate text recognition

- **Performance Metrics**
  - Comparison of detection models based on key metrics

---

## 📂 Dataset

The system was trained on the [Car Plate Detection dataset](https://www.kaggle.com/) from Kaggle, containing:

- 433 vehicle images in PNG format  
- Corresponding annotations in Pascal VOC XML format

---

## 📊 Results

| Model         | mAP@0.5 | mAP@0.5:0.95 | Precision | Recall  |
|---------------|---------|--------------|-----------|---------|
| YOLOv11m      | 0.7860  | 0.4437       | 0.8050    | 0.7727  |
| Faster R-CNN  | 0.9688  | 0.8951       | 0.8951    | 0.7841  |

---

## ⚙️ Usage

1. **Clone the repository**
2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```
3. **Train models** using provided training scripts
4. **Run detection** on your images

---

## 📦 Requirements

- Python 3.8+
- PyTorch
- OpenCV
- Tesseract OCR
- Ultralytics YOLO

---


