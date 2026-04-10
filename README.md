# CNN Visualization: Filters and Feature Maps (CIFAR-10)

## Overview

This project explores the internal workings of Convolutional Neural Networks (CNNs) by visualizing **filters** and **feature maps**. The objective is to understand how CNN models extract and transform image features at different layers.

A CNN model is trained on the CIFAR-10 dataset, and visualization techniques are applied to interpret the learned representations.

---

## Objectives

* Understand how CNNs process images
* Visualize convolutional filters (learned weights)
* Visualize feature maps (layer outputs)
* Analyze hierarchical feature learning in CNNs
* Improve interpretability of deep learning models

---

## Dataset

The model is trained on the **CIFAR-10 dataset**, which contains:

* 60,000 images
* 10 classes
* Image size: 32×32

### Classes

Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck

---

## Project Structure

```
CNN-Visualization-Lab/

├── CNN_Visualization.ipynb
├── requirements.txt
├── README.md
└── results/
    ├── filters.png
    ├── feature_maps_layer1.png
    ├── feature_maps_layer2.png
    └── feature_maps_layer3.png
```

---

## Model Architecture

The CNN model consists of:

* Conv2D (32 filters) → ReLU → MaxPooling
* Conv2D (64 filters) → ReLU → MaxPooling
* Conv2D (128 filters) → ReLU
* Flatten
* Dense (128) → ReLU
* Output Layer (Softmax)

---

## Key Concepts

### Filters (Kernels)

* Learnable weights in convolution layers
* Detect edges, textures, and patterns

### Feature Maps

* Outputs generated after applying filters
* Highlight important regions of the image

### Hierarchical Learning

* Early Layers → Edges, lines
* Middle Layers → Textures, shapes
* Deep Layers → Complex patterns and objects

---

## Implementation Steps

1. Load CIFAR-10 dataset
2. Preprocess images (normalization)
3. Build CNN model
4. Train model
5. Extract filters from convolution layers
6. Visualize filters
7. Generate feature maps using intermediate model
8. Visualize feature maps

---

## Results

| Metric            | Value   |
| ----------------- | ------- |
| Training Accuracy | ~80–85% |
| Test Accuracy     | ~70–80% |

### Visualizations

* Filters capture basic patterns such as edges
* Feature maps show progressive feature extraction

---

## How to Run

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/CNN-Visualization-Lab.git
cd CNN-Visualization-Lab
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Notebook

Open:

```
CNN_Visualization.ipynb
```

Run all cells to:

* Train the model
* Visualize filters
* Visualize feature maps

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Jupyter Notebook

---

## Applications

* Model interpretability
* Debugging neural networks
* Feature understanding in CNNs
* Computer vision research

---

## Key Learnings

* CNNs learn hierarchical representations
* Filters act as pattern detectors
* Feature maps reveal how images are transformed
* Visualization improves understanding of deep learning models

---

## Author

Aparajita Vaish
Computer Vision Lab
253100101
M.Tech

---

## License

This project is for academic purposes only.
