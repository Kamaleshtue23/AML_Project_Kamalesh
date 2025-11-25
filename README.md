# AML_Project_Kamalesh
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
├── notebook/
│   ├── defect_segmentation.ipynb   
├── sample_predictions/
├── paper/
│   └── AML_PROJECT.pdf 
