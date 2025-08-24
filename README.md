# HAM10000 Skin Cancer Classification  
A **beginner-friendly deep learning project** to classify skin lesion images into **7 categories** using **TensorFlow 2.x**, **EfficientNetB0**, and the **HAM10000 dataset**.

---

## **📖 Project Overview**
Skin cancer detection using machine learning can assist dermatologists in early diagnosis and treatment.  
This project uses the **HAM10000 dataset**, which contains **10,015 dermatoscopic images** of skin lesions across **7 classes**.

We fine-tune a **pre-trained EfficientNetB0 model** on the dataset and evaluate performance using **AUC, precision, recall, and F1-score**.

---

## **Dataset**
**Dataset** → [HAM10000 on Kaggle](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)

- **Total Images:** 10,015
- **Classes:**
    - `akiec` → Actinic keratoses  
    - `bcc` → Basal cell carcinoma  
    - `bkl` → Benign keratosis  
    - `df` → Dermatofibroma  
    - `nv` → Melanocytic nevi  
    - `mel` → Melanoma  
    - `vasc` → Vascular lesions
- Each image comes with **metadata**: age, sex, lesion ID, localization, and diagnosis.

---

## **Features**
- Pre-trained **EfficientNetB0** backbone
- **Two-stage training strategy** for better performance  
- Handles **class imbalance** using `class_weight`  
- Uses **tf.data.Dataset** pipeline for faster loading  
- Includes **data augmentation**  
- Generates **classification reports & confusion matrix**  
- Evaluates **melanoma sensitivity** using **precision-recall curves**  
- Integrates **occlusion sensitivity explainability** to see **which regions influence predictions**


---


## Evaluation Metrics

We evaluate performance using multiple metrics:

	•	Accuracy → Overall correctness
	•	AUC (Area Under ROC) → Multi-class separability
	•	Precision → Correct positive predictions
	•	Recall (Sensitivity) → Correctly detected positive cases
	•	F1-Score → Balance between precision & recall

For melanoma detection, recall is prioritized to avoid false negatives.

---

## Visualizations

	•	Training Curves → Loss, Accuracy, and AUC per epoch
	•	Confusion Matrix → Correct vs incorrect classifications
	•	Precision-Recall Curve → Especially for melanoma sensitivity
	•	Occlusion Sensitivity Heatmaps → Visualize regions influencing predictions

---

## Code Structure 

	1.	Environment Setup & Dependencies
	2.	Dataset Downloading & Preparation
	3.	Exploratory Data Analysis (EDA)
	4.	Configuration & Constants
	5.	Train-Validation Split
	6.	TensorFlow Data Pipeline (tf.data)
	7.	Model Building (EfficientNetB0)
	8.	Callbacks & Class Weights
	9.	Model Training: Stage 1 & Stage 2
	10.	Evaluation & Metrics
	11.	Melanoma Sensitivity & PR Curve
	12.	Training Curves Visualization
	13.	Making Predictions on New Images
	14.	Explainability: Occlusion Sensitivity
 
 ## How to use

 - Download HAM10000 dataset from Kaggle
 - Upload in Google Drive 
 - Download the code and run in Google Colab

 ---

 
 ## License

This project is licensed under the MIT License — you’re free to use, modify, and distribute it.
