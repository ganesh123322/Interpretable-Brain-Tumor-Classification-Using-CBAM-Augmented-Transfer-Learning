# BRAIN TUMOR DETECTION AND CLASSIFICATION USING CBAM-AUGMENTED TRANSFER LEARNING

## PROJECT OVERVIEW
This project implements a **deep learning framework** for **automatic brain tumor detection and classification** from MRI images using **attention-enhanced transfer learning**.  
The approach combines a robust **preprocessing pipeline** with **Convolutional Block Attention Modules (CBAM)** integrated into four pre-trained CNN architectures — **ResNet50V2**, **MobileNetV2**, **DenseNet121**, and **EfficientNetB0** — to improve interpretability and accuracy.

## METHODOLOGY
Key preprocessing steps such as **skull stripping**, **contrast enhancement (CLAHE)**, **z-score normalization**, and **data augmentation** ensure cleaner and more consistent MRI inputs.  
Each model is fine-tuned to focus on tumor-relevant features, offering reliable classification across four tumor types:

- Glioma  
- Meningioma  
- Pituitary  
- No Tumor  

---

## STREAMLIT WEB APPLICATION
The web application is built using **Streamlit**, providing an interactive interface for MRI image validation and classification.  
It performs the following functions:

1. Automated preprocessing and validation (to filter non-medical images)  
2. Real-time classification with visual confidence indicators  
3. Support for uploading MRI scans and viewing model predictions instantly  

---

## MODEL FILES
Model weights (`.keras` files) are **not included** in this repository due to GitHub file size limits.  
You can download the trained model files from the following Google Drive link and place them in the `models/` directory:

**Google Drive Link:**  
[https://drive.google.com/drive/folders/1WGPe-S1GKL-jDRf5ivPMTRBoNqe05wmz?usp=drive_link](https://drive.google.com/drive/folders/1WGPe-S1GKL-jDRf5ivPMTRBoNqe05wmz?usp=drive_link)

---

## KEY HIGHLIGHTS
- CBAM-based attention for enhanced interpretability  
- Preprocessing-driven framework to improve MRI quality and model generalization  
- Transfer learning from top ImageNet architectures  
- High classification accuracy (up to 98.78% with MobileNetV2_CBAM)  
- Explainable AI approach using Grad-CAM visualization for interpretability  
- Streamlit-based interactive web interface for deployment  

---

## TECH STACK

| CATEGORY                | TECHNOLOGIES USED |
|----------               |------------------ |
| Programming Language    | Python            |
| Deep Learning Framework | TensorFlow / Keras|
| Image Processing        | OpenCV            |
| Data Analysis           | NumPy, Matplotlib |
| Web Application         | Streamlit         |
| Evaluation Metrics      | scikit-learn      |

---

## MODEL PERFORMANCE

| MODEL NAME         | ACCURACY (%) |
|-------------       |--------------|
| DenseNet121_CBAM   | 98.17 |
| MobileNetV2_CBAM   | 98.78 |
| ResNet50V2_CBAM    | 98.02 |
| EfficientNetB0_CBAM| 96.80 |

---

## HOW TO RUN THE PROJECT

### Step 1: Clone the Repository
```bash
git clone https://github.com/ganesh123322/brain-tumor-detection-cbam.git
cd brain-tumor-detection-cbam
run streamlit run app.py in vs or cmd
