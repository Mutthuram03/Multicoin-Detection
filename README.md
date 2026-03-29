# Multicoin Detection & Counting using YOLOv8

Efficient coin detection and counting from scanned images using deep learning and computer vision.

---

## Overview

This project focuses on automated detection and counting of multiple coins from scanned or captured images using YOLOv8 and OpenCV. It replaces traditional manual counting methods with a fast, accurate, and scalable AI-based solution.

---

## Features

* Detect multiple coins in a single image
* Deep learning-based classification using YOLOv8
* Real-time detection capability
* Accurate coin counting and value estimation
* Handles overlapping coins and complex backgrounds
* Works on both CPU and GPU

---

## Technologies Used

* Python
* OpenCV (image preprocessing)
* YOLOv8 (object detection)
* PyTorch (deep learning framework)

---

## Problem Statement

Manual coin counting is time-consuming, error-prone, and inefficient for large volumes. Mechanical coin counting machines are expensive and not easily accessible.

This project provides an automated, cost-effective solution using computer vision and deep learning.

---

## Methodology

### Traditional Approach (Limitations)

* Grayscale conversion
* Gaussian blur
* Edge detection (Canny)
* Hough Circle Transform

Limitations:

* Poor performance with overlapping coins
* Sensitive to lighting conditions
* Requires manual parameter tuning

---

### Proposed Approach (YOLOv8)

1. Input image
2. Preprocessing using OpenCV
3. YOLOv8 detects coins
4. Bounding boxes and classification
5. Count coins and compute total value

Advantages:

* High accuracy
* Robust to lighting and noise
* Handles overlapping coins
* No manual feature engineering

---

## Model Architecture

* Backbone: Feature extraction (CSPDarknet)
* Neck: Feature fusion (FPN + PAN)
* Head: Detection (class, bounding box, confidence)

---

## Results

* High precision and recall
* Improved detection accuracy compared to traditional methods
* Efficient real-time performance

(Refer to performance graphs in the project report )

---

## Applications

* Banking systems
* Retail checkout automation
* Vending machines
* Coin sorting systems
* Financial applications
* Accessibility tools

---

## Project Structure

```
Multicoin-Detection/
│── dataset/
│── models/
│── runs/
│── detect.py
│── train.py
│── requirements.txt
│── README.md
```

---

## How to Run

### Clone the Repository

```
git clone https://github.com/Mutthuram03/Multicoin-Detection.git
cd Multicoin-Detection
```

### Install Dependencies

```
pip install -r requirements.txt
```

### Train Model (Optional)

```
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50
```

### Run Detection

```
yolo task=detect mode=predict model=best.pt source=images/
```

---

## Future Improvements

* Mobile application integration
* Multi-currency support
* Real-time video detection
* Counterfeit coin detection

---

## Conclusion

This project demonstrates how deep learning and computer vision can automate coin detection and counting efficiently. The use of YOLOv8 significantly improves accuracy, speed, and scalability compared to traditional approaches.

---

## Author

Mutthuram S R

