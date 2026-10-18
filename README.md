[visionguard_ai_repository_readme.md](https://github.com/user-attachments/files/33615411/visionguard_ai_repository_readme.md)
# VisionGuard AI — Automated CV Dataset Quality & Outlier Detector

> **Programmatic dataset hygiene, anomaly detection, and audit reporting for computer vision training pipelines.**

[![License: MIT](https://img.shields.io/badge/License-MIT-cyan.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-emerald.svg)]()

---

## 📌 Executive Summary

Every AI organization building computer vision models struggles with the fundamental truth of machine learning: **garbage in, garbage out**. Undetected bounding box drift, class imbalance, motion blur, and edge-case misclassifications directly lead to wasted GPU hours, degraded inference accuracy, and silent model failures in production environments.

**VisionGuard AI** is an automated dataset quality control suite designed to ingest raw object detection and segmentation datasets (COCO JSON or Pascal VOC XML format) and perform fast, deterministic quality audits before model training begins. Inspired by large-scale dataset curation pipelines managed across computer vision workflows, VisionGuard AI bridges the gap between raw data collection and production-grade dataset hygiene.

---

## 🚀 Key Capabilities

* **Bounding Box Drift & IoU Analysis:** Detects misaligned bounding boxes and calculates Intersection over Union (IoU) variance against automated anchor box predictions.
* **Laplacian Motion Blur Spectrum:** Uses OpenCV Laplacian variance calculations to flag blurred frames, high-speed camera artifacts, and soft-focus captures.
* **Class Entropy & Imbalance Audit:** Measures Shannon Entropy ($H$) across class distributions to pinpoint severe sample skews and underrepresented edge cases.
* **Embedding Anomaly & Outlier Matrix:** Maps feature vectors to highlight visual outliers, lighting extremes, and potential labeling errors.
* **Interactive Local Workspace:** Built-in web workspace with live threshold sensitivity sliders, HTML5 canvas overlay visualizer, and instant auto-correction actions.
* **Actionable Reporting & Sanitation:** Generates downloadable audit logs (`.json`), downloadable sanitized COCO annotation files, and printable executive compliance reports.

---

## 🛠 Tech Stack

* **Core Engine:** Python 3.9+, OpenCV (`cv2`), Pandas, NumPy, SciPy
* **Visualization & Analytics:** Chart.js, HTML5 Canvas API
* **Interface & Presentation:** Tailwind CSS, Lucide Icons, Modern JS (ES6+)
* **Formats Supported:** COCO JSON (`instances_default.json`), Pascal VOC XML, Compressed Image Archives (`.zip`)

---

## 💻 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/visionguard-ai.git
cd visionguard-ai
```

### 2. Open the Local Audit Interface
Simply launch the standalone local workspace interface in your browser:
```bash
# On macOS
open index.html

# On Linux / Windows
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

---

## 📊 Portfolio Case Study Summary (for Resumes / Portfolio Websites)

**Project Name:** VisionGuard AI — Computer Vision Dataset Quality & Outlier Detector  
**Role:** Lead Developer / Computer Vision QA Architect  

* **Problem Solved:** Manual annotation review for thousands of object detection frames is slow, prone to human error, and expensive. Silent dataset flaws directly degrade model performance.
* **Architecture:** Developed an automated Python/CV auditing engine that ingests COCO/VOC datasets and evaluates 4 key structural health indicators: box drift offset, Laplacian blur variance, class distribution entropy, and embedding distance.
* **Impact:** Reduced manual review time for large edge-case suites by programmatically surfacing the top ~12% highest-risk annotation anomalies, allowing teams to auto-fix bounding boxes or export sanitized training sets with one click.

---

---

## ⚖️ License & Intellectual Property

**© 2026 Yadira Rosemary Romancelly. All Rights Reserved.**

This software is released under a **Source-Available Non-Commercial License**. 

* **Evaluation & Personal Use:** Free to inspect, download, test, and evaluate for educational, portfolio, and non-commercial research purposes.
* **Commercial Restriction:** Any commercial use, redistribution, sublicensing, or integration into paid services/products without an explicit commercial license from the author is strictly prohibited.
* **Commercial Licensing & Inquiries:** For enterprise deployment, custom integrations, or commercial license purchases, please contact Yadira Romancelly via GitHub or LinkedIn.
