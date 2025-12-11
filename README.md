# Flair MRI Brain Segmentation using UNet++  

This repository contains a **single Jupyter Notebook**, developed and executed entirely in **Google Colab**, that implements a UNet++ model for segmenting brain regions on FLAIR MRI images.  
The notebook includes the full workflow—from data loading to model training, evaluation, visualization, and exporting model weights.

---

## 📘 Project Overview

The notebook demonstrates how a UNet++ architecture can be applied to medical image segmentation tasks.  
It covers essential deep learning steps including:

- Dataset inspection  
- Preprocessing  
- Defining the UNet++ model in Keras  
- Training the model with MRI data  
- Monitoring performance metrics  
- Visualizing segmentation predictions  

This project serves as a practical, end-to-end example of medical image segmentation using deep learning.

---

## 📄 File Included

### **Flair_MRI_unet++_5.ipynb**
This notebook contains:

### **1. Data Handling**
- Loads MRI image slices and segmentation masks  
- Displays dataset shapes (e.g., `(1373, 256, 256, 1)`)  
- Splits data into **training** and **validation** sets  

### **2. Model Architecture**
- Builds a **UNet++ (Nested U-Net)** model using TensorFlow/Keras  
- Model summary shows approximately **31 million parameters**  
- Designed for binary segmentation on 256×256 FLAIR MRI inputs  

### **3. Training**
- Compiles the model with standard loss and metrics  
- Trains directly in Google Colab  
- Logs:
  - Training loss  
  - Validation loss  
  - Accuracy  
  - Dice coefficient  

### **4. Evaluation & Visualization**
- Plots learning curves for loss and metrics  
- Displays sample predictions, including:
  - Input FLAIR MRI  
  - Ground-truth mask  
  - Predicted mask  

### **5. Model Saving**
- Saves trained weights to a `.h5` file  
- File is **not included** here due to GitHub size limitations  

