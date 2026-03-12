# 🚦 Intelligent Traffic Light Control & Image Processing

A Python + OpenCV simulation of an AI-adaptive traffic intersection 
controller with real-time vehicle detection, congestion analysis, 
and dynamic signal phase management.

## 📌 Features

- 🎥 4 synthetic lane cameras (North, South, East, West)
- 🔍 Vehicle detection using contour-based image processing
- 🚗 Congestion density scoring per lane (0–100%)
- 🚦 4-phase signal cycle (NS Green → NS Yellow → EW Green → EW Yellow)
- 🤖 AI adaptive logic — shortens idle phases when one lane is overloaded
- 📸 Single static snapshot output (no continuous loop)
- 💾 Auto-saves output as traffic_snapshot.png

## 🛠️ Tech Stack

- Python 3.x
- OpenCV (cv2)
- NumPy

## 🚀 Quick Start

pip install opencv-python numpy
python traffic_controller.py

## 📷 Output

A single 1060×480 image combining:
- 2×2 grid of camera feeds with green detection bounding boxes
- Signal control panel with live density bars and system log

## 🧠 Concepts Used

- Binary thresholding & contour detection (cv2.findContours)
- Bounding rectangle extraction (cv2.boundingRect)
- NumPy array image manipulation
- Rule-based AI phase adaptation
- Traffic signal phase logic

## ⌨️ Controls

| Key   | Action          |
|-------|-----------------|
| Any   | Close window    |

## 📁 Structure

├── traffic_controller.py   # Main script (8 cells)
├── traffic_snapshot.png    # Output image (auto-generated)
└── README.md
```
