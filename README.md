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


   🧠 Model & Methodology
🔍 Preprocessing

Resize all MRI images to a uniform size (e.g., 224×224 pixels)

Normalize pixel values to range [0, 1]

Apply data ­augmentation (rotation, shifting, zooming, flipping) on the training set to mitigate overfitting

🏗 Architecture

Base model: e.g., fine-tuned ResNet50 / VGG16 or a custom CNN

Top layers: Dense layers with ReLU activation

Output layer: 4 neurons + Softmax activation (for 4 classes)

Loss function: Categorical Crossentropy

Optimizer: Adam (learning rate: e.g., 1e-4)

📈 Training

To retrain the model from scratch, run:

python main.py


This will:

Load and preprocess the dataset

Train the model

Save the trained weights (in the models/ directory)

🧾 Prediction / Inference

To run inference on a new MRI image, use:

python main.py --predict --image path_to_image.jpg


Output example:

Predicted Class: Pituitary  
Confidence Score: 94.7%

📊 Results & Evaluation

The model was evaluated on an independent test set (not used during training).

Metrics: Accuracy, Precision, Recall, F1-Score.

Confusion matrix and other visualizations can be found in the visualizations/ folder.

📂 Repository Structure
DMBI-Project/
├── data/
│    └── raw/
├── models/
├── visualizations/
├── brain_tumour_detection_using_deep_learning.ipynb
├── main.py
├── requirements.txt
├── README.md
└── LICENSE

👨‍💻 Author

Anish Tawade (GitHub: @Anissh280507
)
