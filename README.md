# 🌴🍎 Palm Tree Detection & Apple Classification

This repository contains my solution to an Artificial Intelligence technical interview assignment. The task focuses on applying computer vision techniques to solve two real-world image problems:

1. **Palm Tree Counting** – Detect and count palm trees in a plantation image using traditional image processing.
2. **Apple Classification** – Detect and crop apples using YOLOv5, and classify them by color (red, yellow, green).

---

## 📁 Repository Contents

- `count.ipynb`  
  Uses OpenCV techniques to detect and count palm trees from `count.jpg`.

- `classify.ipynb`  
  Uses YOLOv5 to detect apples from `classify.jpg`, then classifies them by color using HSV color thresholding.

---

## 🧠 Methods Summary

### 🟩 Palm Tree Detection (`count.ipynb`)
- Libraries: OpenCV, NumPy
- Method:
  - Preprocessing: grayscale, blur, adaptive threshold.
  - Morphological operations to clean noise.
  - Contour detection to find tree locations.
  - Bounding boxes drawn with OpenCV.
  - Sequential numbering added for tree tracking.

### 🟥 Apple Classification (`classify.ipynb`)
- Libraries: Ultralytics YOLOv5, OpenCV, NumPy
- Method:
  - Uses `YOLOv5` from `ultralytics` to detect apples.
  - Each apple is cropped from the image.
  - Apple color is determined by calculating the mean HSV value.
  - Apples are labeled and saved into files like `red_1.jpg`, `green_2.jpg`, etc.

---

## 🛠️ Installation & Setup

### Environment

- Python 3.11+
- Jupyter Notebook
- Ubuntu / macOS (or any UNIX-based system)

### Install dependencies

```bash
pip install opencv-python numpy matplotlib scikit-learn torch torchvision
pip install ultralytics
````

---

## 🚀 Running the Code

### 1. Palm Tree Counting

* Place `count.jpg` in the same folder.
* Open `count.ipynb` in Jupyter.
* Run all cells to generate an annotated image with numbered trees.

### 2. Apple Classification

* Place `classify.jpg` in the same folder.
* Open `classify.ipynb`.
* Run all cells to:

  * Detect apples using YOLOv5.
  * Crop detected apples.
  * Classify each apple as red/yellow/green.
  * Save cropped images with labels (`red_1.jpg`, `green_2.jpg`, etc.)

---

## 📌 Attribution

**Image sources (as per assignment):**

* Palm trees:
  [https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai\_assignment\_20241202\_count.jpeg](https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai_assignment_20241202_count.jpeg)

* Apples:
  [https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai\_assignment\_20230726\_classify.jpeg](https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai_assignment_20230726_classify.jpeg)

**Libraries Used:**

* [OpenCV](https://opencv.org/)
* [Ultralytics YOLOv5](https://github.com/ultralytics/ultralytics)
* [NumPy](https://numpy.org/)
* [PyTorch](https://pytorch.org/)

---

## 📄 License

This project is intended for educational and technical evaluation purposes.
