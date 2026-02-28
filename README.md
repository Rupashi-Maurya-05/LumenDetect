🌙 LumenDetect

Analysis of Object Detection Models under Low-Light Environments

📌 Overview

LumenDetect is a comparative study of state-of-the-art object detection models evaluated under challenging low-light conditions. The project benchmarks model robustness without enhancement and after applying contrast enhancement techniques.

🎯 Objectives

Evaluate detection performance in real-world dark environments

Compare one-stage and two-stage detectors

Analyze the impact of image enhancement on detection accuracy

Establish robustness benchmarks for illumination-aware systems

📂 Dataset

Dataset: ExDark

7,363 real-world low-light images

12 object categories

Evaluation subset: 2,405 images (Bottle, Chair, Cup, Dog, Table)

🤖 Models Evaluated

YOLOv5

SSD (Single Shot Detector)

Faster R-CNN

🧪 Methodology
Phase 1 – Baseline

Models tested on raw low-light images

No enhancement applied

Phase 2 – Enhancement-Based

Applied CLAHE (Contrast Limited Adaptive Histogram Equalization)

Compared performance under identical training/testing conditions

📊 Evaluation Metrics

Precision

Recall

F1-Score

mAP@0.5

mAP@0.5–0.95

Inference Time (ms/image)

📈 Key Results
🔹 YOLOv5

F1 Score: 0.72 → 0.75

Inference Time: 531 ms → 522 ms (CPU)

Overall mAP@0.5: 76.3% → 79.7% (+3.4%)

🔹 Enhancement Impact (Overall)

mAP@0.5: +3.4%

mAP@0.5–0.95: +2.9%

Recall: +6.1%

Precision: +2.4%

🔹 SSD Baseline

mAP@0.5: 64.7%

Recall: 96.4%

F1 Score: 0.77

🏆 Key Insights

Enhancement improves recall significantly in dark scenes

One-stage detectors show strong speed-performance tradeoff

Performance varies across object classes (Table class improved by +8.3%)

Low-light robustness requires both architectural strength and preprocessing

🚀 Future Scope

Evaluate on larger low-light datasets

Test advanced enhancement methods (Retinex, GAN-based)

Optimize for real-time GPU deployment

Integrate illumination-aware training strategies

👩‍💻 Authors

Rupashi Maurya
Muskan Kumari

Supervisor: Mrs. Manushree
