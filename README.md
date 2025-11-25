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

text
.
├── README.md
├── notebook/
│   ├──  Segmentation Pipeline.ipynb   
├── sample_predictions/
├── paper/
│   └── AML_PROJECT.pdf

## Google Colab Notebook

Due to the large size of the `.ipynb` file (including all outputs, debugging runs, images, and activation visualizations), the full training notebook is hosted on Google Colab:

**🔗 Notebook Link: https://colab.research.google.com/drive/1XXEzsj0ou3yl7l0fdW0N0mmy5SKmqSOA?usp=sharing**

This contains:
- dataset preparation
- augmentation pipeline
- model implementations
- training loops
- evaluation metrics
- visualization of predictions
- feature activation analysis
- 
## 🔗 Benchmark Dataset Link: https://drive.google.com/drive/folders/1YmFu23_RppdlG5w5H-psU8E-bhMv8Qib?usp=sharing


## 🔗 CVAR Annotated Augmented Dataset Link: https://drive.google.com/drive/folders/1PuP2hW7tY45xZFcoqd66CNUb_4Zf-aPP?usp=sharing

