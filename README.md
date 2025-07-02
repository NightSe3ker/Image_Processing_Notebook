# 🖼️ Image Processing & OCR with OpenCV and Tesseract

This project demonstrates the use of **OpenCV** for basic image processing tasks and **Tesseract OCR** for extracting text from images. It covers both traditional computer vision techniques and optical character recognition using pre-trained tools.

---

## ✅ What This Project Does

This notebook performs the following key tasks:

### 🔍 1. Edge Detection
- Uses **convolution filters** and **custom kernels** (like the Sobel filter) to identify edges in images.
- Demonstrates how edge detection highlights vertical, horizontal, or diagonal features.
- Explains the difference between OpenCV filters and deep learning kernels (which are learned vs. manually set).

### ⚡ 2. Canny Edge Detection
- Implements OpenCV’s built-in `cv2.Canny()` function.
- Provides more refined, noise-reduced edge detection using automatic thresholds and gradient intensity.
- Useful for preparing images for further processing like segmentation or OCR.

### 🧾 3. Optical Character Recognition (OCR)
- Extracts text from images using the **Tesseract** engine via the `pytesseract` wrapper.
- Starts with a simple image and shows how text is extracted easily.
- Then applies the same OCR process to a complex or noisy image, which initially fails.

### 🛠️ 4. Image Preprocessing for OCR
To improve OCR results on difficult images, the following preprocessing steps are applied:
- **Grayscale conversion**: Simplifies color info into intensity levels.
- **Thresholding**: Binarizes the image (black & white) to improve text clarity.
- **Noise removal**: Removes irrelevant pixels to clean the image.
- **Image scaling**: Increases resolution to improve character recognition.

These steps demonstrate how preprocessing enhances OCR accuracy significantly.

### 🖼️ 5. Visualization
- Custom plotting functions are used to display:
  - Original images
  - Filtered/processed versions
  - OCR results
- Helpful for comparing effects of different techniques visually.

---

## 🛠️ Technologies Used

| Tool / Library     | Purpose                                      |
|--------------------|----------------------------------------------|
| **Python**         | Programming language                         |
| **OpenCV** (`cv2`) | Image processing: filtering, edges, resize   |
| **Pytesseract**    | OCR using Google's Tesseract engine          |
| **Matplotlib**     | Visualization of image outputs               |
| **NumPy**          | Array operations on image data               |

---

## 🧠 Concepts Demonstrated

- Classical image filtering (with static kernels)
- Difference between Deep Learning and traditional filters
- Canny edge detection algorithm
- OCR challenges and preprocessing solutions
- Text extraction workflow using `pytesseract`

---

## 🚀 Use Cases

- **Text extraction** from scanned documents, receipts, or signboards
- **Preprocessing pipeline** for OCR and document digitization
- **Visual analysis** of how image filters transform data
- **Educational demo** for beginners in computer vision and OCR

---

## 📋 Requirements

To run this notebook, install the following:

```bash
pip install opencv-python pytesseract numpy matplotlib
