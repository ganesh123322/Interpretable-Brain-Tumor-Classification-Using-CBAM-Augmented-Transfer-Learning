This project implements a deep learning framework for automatic brain tumor detection and classification from MRI images using attention-enhanced transfer learning. The approach combines a robust preprocessing pipeline with Convolutional Block Attention Modules (CBAM) integrated into four pre-trained CNN architectures — ResNet50V2, MobileNetV2, DenseNet121, and EfficientNetB0 — to improve interpretability and accuracy.

Key preprocessing steps such as skull stripping, contrast enhancement (CLAHE), z-score normalization, and data augmentation ensure cleaner and more consistent MRI inputs.
Each model is fine-tuned to focus on tumor-relevant features, offering reliable classification across four tumor types: glioma, meningioma, pituitary, and no tumor.

The web application is built with Streamlit, providing an interactive interface for MRI image validation and classification. It performs:

Automated preprocessing and validation (to filter non-medical images),

Real-time classification with visual confidence indicators,

Support for uploading MRI scans and viewing model predictions instantly.

⚠️ Model weights (.keras files) are not included due to size limits. You can download them from external links provided in the README.

🔍 Highlights

🧩 CBAM-based attention for enhanced interpretability

🧠 Preprocessing-driven framework to improve MRI quality and model generalization

🧰 Transfer learning from top ImageNet architectures

📊 High classification accuracy (up to 98.78% with MobileNetV2_CBAM)

💡 Explainable AI approach using Grad-CAM visualization for attention insight

🌐 Streamlit web app for easy deployment and interactive inference

📦 Tech Stack

Python, TensorFlow/Keras, OpenCV, NumPy, Matplotlib

Streamlit for the interactive web UI

scikit-learn for evaluation metrics and confusion matrices
