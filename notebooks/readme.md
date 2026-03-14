# Notebooks

This directory contains Jupyter notebooks used for training, evaluation, and visualization in the pediatric wrist fracture analysis.

## Overview

The notebooks implement the deep learning pipeline for fracture analysis from wrist radiographs. The workflow includes:

1. Fracture detection using YOLOv11
2. Fracture AO subtype classification using ConvNeXt
3. Model evaluation and performance comparison
4. Explainable AI visualization using XAI techniques

## Execution Environment

The notebooks were executed using the Kaggle platform with GPU support.

Key libraries used:

* PyTorch
* Ultralytics YOLO
* NumPy
* OpenCV
* Matplotlib
* Scikit-learn

## Notes

* Model weights generated from training are stored in the `models` directory.
* Dataset paths may need modification when running locally.
* GPU acceleration is recommended for training and inference.
