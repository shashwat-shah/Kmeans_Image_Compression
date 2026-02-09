# Kmeans_Image_Compression

This repository demonstrates **image compression using the K-Means clustering algorithm**.  
The project shows how unsupervised learning can be applied to reduce the number of colors in an image while preserving its overall visual structure.

This is a learning-oriented implementation intended to illustrate the concept rather than a production-ready system.

---

## Overview

Images consist of pixels represented by RGB color values. Instead of storing every unique pixel color, K-Means clustering groups similar colors into **k clusters**. Each pixel is then replaced by the centroid of its cluster, resulting in a compressed image.

Reducing the value of *k* increases compression but lowers image quality, while increasing *k* improves quality at the cost of higher storage.

---

## Approach

1. Load an input image
2. Reshape the image into a 2D array of RGB pixel values
3. Apply K-Means clustering to group pixels into *k* clusters
4. Replace each pixel with its cluster centroid
5. Reconstruct and display the compressed image

Example

k = 8 → High compression, lower visual quality

k = 16 → Balanced compression and quality

k = 32+ → Better quality, lower compression


### Dependencies

Python 3.x

numpy

matplotlib

scikit-learn

Pillow (PIL)

jupyter
