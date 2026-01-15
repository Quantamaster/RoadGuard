

---

# 🛣️ RoadGuard — AI-Powered Road Distress Detection

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python\&logoColor=white)
![AI](https://img.shields.io/badge/AI-Computer%20Vision-orange)
![SAM](https://img.shields.io/badge/Model-Segment%20Anything-green)
![License](https://img.shields.io/badge/License-MIT-purple)

**RoadGuard** is an AI-driven road infrastructure monitoring system designed to automatically detect and segment road distresses (such as potholes) using computer vision and deep learning.
It supports **geo-tagged detection**, **mask-based visualization**, and is designed for **web & mobile deployment**.

---

## 📑 Table of Contents

* [About the Project](#-about-the-project)
* [Problem Statement](#-problem-statement)
* [Solution Overview](#-solution-overview)
* [Key Features](#-key-features)
* [Tech Stack](#-tech-stack)
* [System Architecture](#-system-architecture)
* [Model & Methodology](#-model--methodology)
* [Installation](#-installation)
* [Usage](#-usage)
* [Results & Outputs](#-results--outputs)
* [Applications](#-applications)
* [Future Improvements](#-future-improvements)
* [Run and Deploy your AI Studio App](#-run-and-deploy-your-ai-studio-app)



---

## 📌 About the Project

Road infrastructure degradation is a major challenge for transportation authorities. Manual inspection is **slow, expensive, and error-prone**.

**RoadGuard** leverages **AI & ML** to:

* Detect road surface damage
* Segment potholes using masks
* Store **GPS-based location data**
* Enable scalable road condition monitoring

---

## ❗ Problem Statement

Traditional road inspection methods:

* Require manual surveys
* Are not scalable
* Lack real-time insights
* Miss early-stage deterioration

---

## 💡 Solution Overview

RoadGuard provides an **automated AI solution** that:

1. Takes road images or video frames
2. Detects distress regions
3. Segments potholes using **Segment Anything Model (SAM)**
4. Saves geo-coordinates for mapping and maintenance planning

---

## ✨ Key Features

* 🚧 **AI-based road distress detection**
* 🎯 **Mask-level segmentation of potholes**
* 📍 **Latitude & longitude tagging**
* 🖥️ **Web & mobile-friendly architecture**
* 📊 **Visual overlays for severity estimation**

---

## 🧰 Tech Stack

| Layer           | Technology                   |
| --------------- | ---------------------------- |
| Language        | Python                       |
| Computer Vision | OpenCV                       |
| Deep Learning   | Segment Anything Model (SAM) |
| Frontend        | TypeScript / React           |
| Backend         | Python (ML inference)        |
| Mapping         | GPS coordinates              |

---

## 🏗️ System Architecture

```
Input Image / Video
        ↓
AI Detection Model
        ↓
SAM Segmentation
        ↓
Mask Overlay + Geo-Tagging
        ↓
Web / Mobile Visualization
```

---

## 🧠 Model & Methodology

* **Detection Stage**
  Identifies road distress regions from images.

* **Segmentation Stage**
  Uses **Segment Anything Model (SAM)** to extract precise pothole boundaries.

* **Post-Processing**

  * Mask visualization
  * Area estimation
  * Location tagging

---

## ⚙️ Installation

```bash
git clone https://github.com/Quantamaster/RoadGuard.git
cd RoadGuard
```

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

```bash
python main.py
```

* Provide road images or video frames
* Model outputs segmented pothole masks
* Location data is stored for mapping

---

## 📊 Results & Outputs

* ✔ Accurate pothole segmentation
* ✔ Mask-based visual overlays
* ✔ Geo-referenced road distress points
* ✔ Ready for integration with GIS dashboards

---

## 🌍 Applications

* Smart city infrastructure monitoring
* Highway maintenance planning
* Road safety analysis
* Automated inspection systems
* Government & municipal agencies

---

## 🚀 Future Improvements

* Real-time video stream inference
* Severity scoring & prioritization
* GIS dashboard integration
* Edge deployment (mobile devices)
* Multi-class road defect detection

---

<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

## 🚀 Run and Deploy your AI Studio App

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1tGdz-pSLCFx9TQlYB64oAhsblhRGXGrF

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`
