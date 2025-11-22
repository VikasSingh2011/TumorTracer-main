# TumorTracer 🧠

TumorTracer is an AI-powered brain tumor detection system that classifies MRI scans into “tumor” or “non-tumor” using deep learning. It leverages a Convolutional Neural Network (CNN) trained on pre-processed MRI data and provides interpretable results with high accuracy.

## 🚀 Key Features

- Pre-processes and augments 3,000+ MRI scans (resizing, normalization, flips, rotations)  
- CNN-based architecture with dropout and dense layers  
- Training visualization: accuracy & loss curves  
- Confusion matrix for validation on a 15% hold-out set  
- Final model achieves **94% accuracy**

## 📁 Dataset & Pre-processing

1. Load raw MRI images (binary or grayscale)  
2. Resize images to a fixed dimension (e.g., 150×150)  
3. Normalize pixel intensities  
4. Perform data augmentation (rotation, flip, zoom) to increase generalization  
5. Split dataset into **training**, **validation** (15%), and **test** sets  

## 🧠 Model Architecture

- Several **Conv2D** + **ReLU** layers for feature extraction  
- **MaxPooling** layers to reduce spatial size  
- **Dropout** layers for regularization  
- Flatten + Dense layers for classification  
- Final output: 1 neuron (sigmoid) for binary classification

## 📊 Training Details

- **Loss**: Binary cross-entropy  
- **Optimizer**: Adam  
- **Metrics**: Accuracy  
- **Epochs / Batch Size**: *(specify in your code)*  
- **Validation**: Uses 15% validation split  
- **Callbacks**: (optional) Model checkpoint, early stopping

## 🔍 Evaluation & Results

- Plot training vs validation **accuracy** and **loss** curves  
- Generate a **confusion matrix** for the validation set  
- Calculate **precision** / **recall**  
- Interpret whether the model is overfitting or underfitting

## ⚙️ How to Run Locally

1. Clone the repo  
   ```bash
   git clone https://github.com/VikasSingh2011/TumorTracer-main/blob/main/README.md
   cd TumorTracer-main
