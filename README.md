# DS4002-MI3-Project3
MI3 Repository - Group 7

## Predicting ASL Digit Signs from Images

### **Contents of this repository**
This repository contains our code, data, and output for our ASL digit sign classification project. The goal was to train a convolutional neural network (CNN) to recognize American Sign Language (ASL) digits (0–9) from static hand sign images. This project was completed as part of **DS 4002 (Data Science Project Course)** at the University of Virginia.

---

## **1. Software and Platform**

- **Software:** Python  
- **Packages Used:**  
  - `tensorflow`  
  - `numpy`  
  - `matplotlib`  
  - `sklearn`  
  - `keras`  
  - `glob`  
  - `os`
---

## **2. Documentation Map**

📂 **Root Directory**  
- `README.md` → This documentation file  
- `LICENSE.md` → MIT License  

📂 **DATA/**  
- `palceholder` → Dataset of ASL digit images (`0-9` subfolders)

📂 **SCRIPTS/**  
- `ASL_Digit_CNN_Analysis.ipynb` → Main Colab notebook used to run the analysis

📂 **OUTPUT/**  
- `model_accuracy_plot.png` → Accuracy graph (train/val)  
- `confusion_matrix.png` → Visualized confusion matrix  
- `classification_report.png` → Model performance report  
- `asl_digit_model.h5` → Saved CNN model weights

---

## **3. Instructions for Reproducing CNN Results**

> These steps will reproduce the full model training and evaluation pipeline using Google Colab.

1. **Open** the notebook `01_Perform_ASL_Digit_CNN_Analysis.ipynb` in Google Colab.
2. **Mount Google Drive** (you'll be prompted when you run the first cell).
3. **Ensure the dataset is stored** in:  
   `/MyDrive/Sign-Language-Digits-Dataset/Dataset/` with subfolders `0` through `9`, each containing `.JPG` images.
4. **Run all cells** in order. The notebook will:
   - Load and normalize the images
   - Encode labels as categorical
   - Split data into training and testing sets (75/25)
   - Build a CNN with convolution, pooling, dropout, and dense layers
   - Train the model for 15 epochs
   - Evaluate the model on the test set
   - Output performance metrics (accuracy, confusion matrix, F1 scores)
   - Save the model and figures to the OUTPUT folder

---

## **4. Citations**

### Data Source  
- https://github.com/ardamavi/Sign-Language-Digits-Dataset

### Tools & Resources  
- https://chatgpt.com/share/67fdd7bc-3414-8004-b10d-9ff1e03df96c  
- TensorFlow + Keras Documentation  
- Google Colab environment  
- Project TIER Protocol: https://www.projecttier.org/tier-protocol/protocol-4-0

---

## **5. Summary**

This project aims to create a product that can reliably and accurately predict which ASL digit is being signed based on a static image of that sign. In this project, we:
- Obtained a dataset of approximately 2180 images of ASL digit signs (0-9), signed by different people.
- Transferred that dataset to Google Drive and created a machine learning algorithm in Python using CNN (Convolutional Neural Networks) to analyze the images.
- After training the CNN model on 75% of the data, we tested our model on the remaining 25% of the data.
- We then studied the performance of our model using the standard metrics (accuracy, F1 scores, a confusion matrix, etc).

Overall, we were able to create a model that can accurately classify signs from 75-95% accuracy, depending on the sign. These results highlight the possible ways to use machine learning methods to bridge cross-cultural communication gaps and improve our understanding of other languages - including signed languages like ASL. 

**Team 7, The Unsupervised Learners – DS 4002**
