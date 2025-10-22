# 🧠 Brain Tumor Detection & Classification using MRI  
*(DMBI-Project)*

This repository presents a **deep-learning solution** for the **automated detection and classification** of brain tumors using MRI scans. The model is trained and validated on the Brain Tumor MRI Dataset (sourced from Kaggle) and classifies each input image into one of four categories:  
- **Glioma**  
- **Meningioma**  
- **Pituitary**  
- **No Tumor**

This tool can assist medical professionals in preliminary diagnostics by providing a fast, reliable classification of MRI images.

---

## 📊 Project Overview  

| Item                 | Description                                                         |
|----------------------|---------------------------------------------------------------------|
| **Task**             | Multi-class image classification                                    |
| **Dataset**          | Brain Tumor MRI images (from Kaggle)                                |
| **Target Classes (4)**| Glioma, Meningioma, Pituitary, No Tumor                            |
| **Model Architecture**| Custom CNN (or fine-tuned backbone such as ResNet50/VGG16)         |
| **Metrics**          | Accuracy, Precision, Recall, F1-Score                                                        |

---

## 🚀 Getting Started  

### 🧩 Prerequisites  
- Python 3.8 or higher  
- NVIDIA GPU with CUDA support (recommended for faster training)  
- Virtual environment (optional but recommended)  

### ⚙️ Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Anissh280507/DMBI-Project.git
   cd DMBI-Project
