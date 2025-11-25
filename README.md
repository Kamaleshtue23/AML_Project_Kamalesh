# AML_Project_Kamalesh
# File: README.md
# =================
# Defects Detection in Electroluminescence Images of PV Modules
#
# Git repo for the project:
# "Defects Detection in Electroluminescence Images of Photovoltaic Modules
#  Using Deep Semantic Segmentation"

# ------------------ README.md ------------------
# Defects Detection in Electroluminescence Images of Photovoltaic Modules
# Using Deep Semantic Segmentation

This repository contains the code and artefacts for the project:

> **Defects Detection in Electroluminescence Images of Photovoltaic Modules Using Deep Semantic Segmentation**

It implements three semantic segmentation models:

1. **U-Net** with **ResNet-50** encoder  
2. **DeepLabV3+** with **Xception** backbone  
3. **DeepLabV3+** with **ResNet-101** backbone  

The models are trained and evaluated on:

- A **benchmark EL dataset** (Pratt et al. [1])  
- A **custom CVAT-annotated dataset** (124 cells, 7 classes)  

The accompanying report is in `paper/AML_PROJECT.pdf`.

---

## 1. Repository Structure

```text
.
├── README.md
├── requirements.txt
├── data/
│   ├── cvat/
│   │   ├── images/      # EL cell images (.png / .jpg)
│   │   └── masks/       # class-indexed masks (same filenames as images)
│   └── benchmark/
│       ├── images/
│       └── masks/
├── checkpoints/
│   └── (models will be saved here)
├── src/
│   ├── __init__.py
│   ├── train.py
│   ├── eval.py
│   ├── datasets/
│   │   ├── __init__.py
│   │   └── el_dataset.py
│   ├── models/
│   │   ├── __init__.py
│   │   └── factory.py
│   └── utils/
│       ├── __init__.py
│       ├── losses.py
│       ├── metrics.py
│       └── transforms.py
└── paper/
    └── AML_PROJECT.pdf  # your final report (copy it here)
