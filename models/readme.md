# Models

This directory contains the trained deep learning models used for pediatric wrist fracture detection and classification from X-ray images.

## Overview

Two main models are used in this project:

* **YOLOv11** – used for detecting fracture regions in pediatric wrist radiographs.
* **ConvNeXt** – used for classifying fracture subtypes after region detection.

These models work together to perform automated fracture analysis.

---

## Available Models

| Model    | Task                                         | File                 |
| -------- | -------------------------------------------- | -------------------- |
| YOLOv11  | Fracture region detection (object detection) | `yolov11_best.pt`    |

Download the trained classification model from the link below:
[ConvNeXt Model](https://drive.google.com/file/d/1D18EpsBaRYztRzazJ3PjMMvN7cibfWf_/view?usp=sharing)

---

## YOLOv11 – Fracture Detection

YOLOv11 is used to detect fracture regions in wrist X-ray images.
It performs **object detection** by predicting bounding boxes around fracture locations.

## ConvNeXt – Fracture Classification

ConvNeXt is used to classify the detected fracture regions into different fracture categories.

## Workflow

The complete pipeline works as follows:

1. Input wrist X-ray image
2. YOLOv11 detects fracture regions
3. Detected regions are cropped
4. ConvNeXt classifies the fracture type

## Notes

* Only the best-performing trained weights are stored in this folder.
* Ensure the required dependencies are installed before loading the models.
* Training codes are located in the `notebooks` directory.
