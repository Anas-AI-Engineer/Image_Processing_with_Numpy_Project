# 🖼️ Advanced Image Processing with NumPy

A Python-based image processing project focused on image loading, pixel-level analysis, and visualization using **NumPy, Matplotlib, and Pillow**.

This project explores how digital images are represented as numerical arrays and how NumPy can be used to analyze image properties efficiently.

## 📌 Project Overview

Digital images consist of pixels, and each pixel contains numerical intensity values. Using NumPy, we can convert images into arrays and perform mathematical operations to understand their structure and properties.

The goal of this project is to build a strong foundation in image processing and computer vision through practical Python programming.

## ✨ Features

- 🖼️ Load images using Pillow (PIL)
- 🔢 Convert RGB images into NumPy arrays
- 📐 Analyze image shape and dimensions
- 🎨 Inspect RGB image data
- 📊 Calculate minimum, maximum, and average pixel values
- 👁️ Visualize images using Matplotlib
- 📝 Document code with explanatory comments

## 🛠️ Technologies Used

- **Python** — Core programming language
- **NumPy** — Array operations and numerical analysis
- **Matplotlib** — Image visualization
- **Pillow (PIL)** — Image loading and RGB conversion
- **Jupyter Notebook** — Interactive development and experimentation

## 📂 Project Structure

```text
advanced-image-processing-numpy/
│
├── image_processing.ipynb
├── sample.png
└── README.md
```

## ⚙️ Installation

Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/advanced-image-processing-numpy.git
```

Navigate to the project directory:

```bash
cd advanced-image-processing-numpy
```

Install the required libraries:

```bash
pip install numpy matplotlib pillow
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `image_processing.ipynb` and run the cells.

## 🚀 Current Implementation

The current version loads a sample RGB image, converts it into a NumPy array, calculates basic pixel statistics, and displays the image using Matplotlib.

Example:

```python
import numpy as np
import matplotlib.pyplot as plt
from PIL import Image

img = Image.open("sample.png").convert("RGB")
image = np.array(img)

print("Image Shape:", image.shape)
print("Image Dimensions:", image.ndim)
print("Data Type:", image.dtype)
print("Minimum Pixel:", image.min())
print("Maximum Pixel:", image.max())
print("Average Pixel:", image.mean())

plt.figure(figsize=(10, 6))
plt
