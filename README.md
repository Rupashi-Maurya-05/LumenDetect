# 🌙 LumenDetect  
### Analysis of Object Detection Models under Low-Light Environments

LumenDetect is a comparative study evaluating state-of-the-art object detection models under challenging low-light conditions. The project benchmarks model robustness on raw dark images and after applying contrast enhancement.

---

## 🚀 Project Highlights

- Evaluated **YOLOv5, SSD, Faster R-CNN**
- Tested on **ExDark dataset (7,363 images, 12 classes)**
- Evaluated subset of **2,405 low-light images**
- Applied **CLAHE enhancement**
- Achieved **+3.4% mAP@0.5** improvement after enhancement

---

## 📂 Dataset

**ExDark Dataset**
- 7,363 real-world low-light images
- 12 object categories
- Bounding box annotations
- Illumination metadata

Evaluation classes used:
- Bottle
- Chair
- Cup
- Dog
- Table

---

## 🤖 Models Compared

- YOLOv5 (One-stage detector)
- SSD (Single Shot Detector)
- Faster R-CNN (Two-stage detector)

---

## 🧪 Methodology

### Phase 1 – Baseline
- Tested models on raw low-light images
- No preprocessing applied

### Phase 2 – Enhancement
- Applied CLAHE (Contrast Limited Adaptive Histogram Equalization)
- Re-evaluated under identical training/testing conditions

---

## 📊 Evaluation Metrics

- Precision
- Recall
- F1-Score
- mAP@0.5
- mAP@0.5–0.95
- Inference Time (ms/image)

---

## 📈 Key Results

### 🔹 YOLOv5
- F1 Score: **0.72 → 0.75**
- Inference Time: **531 ms → 522 ms (CPU)**
- mAP@0.5: **76.3% → 79.7% (+3.4%)**

### 🔹 Overall Enhancement Impact
- mAP@0.5: **+3.4%**
- mAP@0.5–0.95: **+2.9%**
- Recall: **+6.1%**
- Precision: **+2.4%**
- Table class improvement: **+8.3%**

### 🔹 SSD Baseline
- mAP@0.5: **64.7%**
- Recall: **96.4%**
- F1 Score: **0.77**

---

## 🏗 Tech Stack

- Python
- PyTorch
- OpenCV
- Matplotlib
- NumPy

---

## 📌 Key Insights

- Low-light conditions significantly impact detection reliability
- Enhancement improves recall more than precision
- One-stage models offer strong speed–accuracy tradeoff
- Class-wise performance varies significantly under illumination shifts

---

## 👩‍💻 Authors

- Rupashi Maurya  
- Muskan Kumari  

**Supervisor:** Mrs. Manushree  
MCA – IT Department  

---

## 📌 Future Work

- Evaluate additional enhancement techniques (Retinex, GAN-based)
- GPU optimization for real-time deployment
- Illumination-aware training strategies
