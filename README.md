# 🌴🍎 Palm Tree Detection & Apple Classification

This repository contains my solution for a assignment focused on applying computer vision to real-world problems in agriculture. The task was divided into two parts:

1. **Palm Tree Counting** – Automatically detect and count palm trees in a plantation image.
2. **Apple Classification** – Identify and crop apples from an image and classify them by color: red, yellow, or green.

---

## 📁 Repository Structure

- `count.ipynb`  
  Detects and counts individual palm trees from `count.jpg`, drawing bounding boxes with sequential numbering.

- `classify.ipynb`  
  Detects apples from `classify.jpg`, classifies their color (red, yellow, green), and exports cropped images (e.g., `red_1.jpg`, `yellow_2.jpg`, etc.).

---

## 🛠️ Installation & Setup

To run these notebooks, you will need:

- Python 3.11+
- Jupyter Notebook

### Install dependencies:

```bash
pip install opencv-python numpy matplotlib scikit-learn
````

You may also need:

```bash
pip install imutils
```

---

## 🚀 Running the Code

### 1. **Palm Tree Counting**

* Place `count.jpg` (plantation image) in the same folder.
* Open `count.ipynb` in Jupyter.
* Run all cells to:

  * Detect palm trees.
  * Generate an output image with bounding boxes and sequential numbers.

### 2. **Apple Classification**

* Place `classify.jpg` (apples image) in the same folder.
* Open `classify.ipynb` in Jupyter.
* Run all cells to:

  * Detect apples.
  * Classify their color using average HSV values or a trained color model.
  * Crop and save each apple image as `red_1.jpg`, `yellow_1.jpg`, etc.

---

## 📊 Techniques Used

### ✅ Palm Tree Counting

* Preprocessing with OpenCV
* Contour detection / blob analysis
* Bounding box drawing and indexing

### ✅ Apple Classification

* Color space transformation (BGR → HSV)
* KMeans clustering or threshold-based color classification
* Image cropping and export

---

## 📌 Attribution

Sample image references (provided in the assignment):

* Palm tree image:
  [https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai\_assignment\_20241202\_count.jpeg](https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai_assignment_20241202_count.jpeg)

* Apple image:
  [https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai\_assignment\_20230726\_classify.jpeg](https://storage.googleapis.com/648010c1-f244-4641-98f2-73ff6c1b4e99/ai_assignment_20230726_classify.jpeg)

Used libraries:

* [OpenCV](https://opencv.org/)
* [NumPy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [Scikit-learn](https://scikit-learn.org/)

---

## 📄 License

This project is for educational and demonstration purposes.
