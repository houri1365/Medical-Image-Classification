# 🩺 Medical Image Classification
## **Diabetic Retinopathy Detection by Deep Learning Classifiers**

> *"Imagine being able to detect blindness before it happens."*


> ### 📖 Overview

Millions of people worldwide suffer from **diabetic retinopathy (DR)** — the leading cause of preventable blindness among working-aged adults.

This project applies **deep learning classifiers** to automatically detect and classify diabetic retinopathy from **retinal fundus images**, aiming to assist early diagnosis and intervention. It also uses Grad_CAM to explore the inner function of different deep learning models.
---

### 🧠 Project Description
The dataset consists of **retina scan images** labeled according to the severity of diabetic retinopathy. All images have been **resized to 224×224 pixels** for compatibility with popular pre-trained deep learning architectures.

Each image is categorized into one of **five severity classes**:

| Label | Class Name        | Description                    |
|-------|-------------------|--------------------------------|
| 0     | No_DR             | No diabetic retinopathy        |
| 1     | Mild              | Mild non-proliferative DR      |
| 2     | Moderate          | Moderate non-proliferative DR  |
| 3     | Severe            | Severe non-proliferative DR    |
| 4     | Proliferate_DR    | Proliferative diabetic retinopathy |
---

### 🧬 Dataset Information

Type : Retinal fundus photography  
Imaging Device : Fundus camera (visible-light ophthalmic camera)  
Modality Category: Optical / Photographic Imaging  
Image Type: 2D color RGB images

---

**Source & Details:**
- **Dataset:** APTOS 2019 Blindness Detection (resized to 224x224).  
- **Kaggle competition:** Diabetic Retinopathy Detection (EyePACS).  
- **Link:** https://www.kaggle.com/datasets/sovitrath/diabetic-retinopathy-224x224-2019-data  
- **Dataset Size:** 3,662 images (JPEG + CSV labels).  
- **Labels:** 0–4 (No DR → Proliferative DR).
---

  ### ⚙️ Models & Performance

| Model            | Accuracy | Macro F1 | Weighted F1 | No_DR F1 | Mild F1 | Moderate F1 | Severe F1 | Proliferative F1 |
|------------------|-----------:|---------:|------------:|---------:|--------:|-----------:|---------:|-----------------:|
| **ResNet-50**     | 75.27%    | 0.33    | 0.67        | 0.97    | 0.00   | 0.70      | 0.00    | 0.00            |
| **EfficientNet-V2** | 82.49%    | 0.66    | 0.82        | 0.98    | 0.64   | 0.76      | 0.45    | 0.47            |
| **MobileNet-V4**   | 79.96%    | 0.61    | 0.80        | 0.98    | 0.51   | 0.73      | 0.40    | 0.44            |
| **ViT-Base**       | 81.05%    | 0.62    | 0.80        | 0.98    | 0.60   | 0.79      | 0.24    | 0.56            |
| **DeiT-III**       | **83.00%** | **0.68**| **0.83**    | **0.98**| **0.62**| **0.77**  | **0.42**| **0.60**        |

**Key notes:** Transformer-based models (DeiT/ViT) and EfficientNet variants tend to perform best. Class imbalance affects detection of minority classes (Mild, Proliferative).

---

### 🧩 Key Insights
- Transformer-based models (DeiT, ViT) outperform traditional CNNs in multi-class DR classification.
- EfficientNet-V2 offers a strong balance between accuracy and computational efficiency.
- Class imbalance is a major challenge, particularly for Mild and Proliferative DR stages.
---

### 💡 Applications
- Early detection and screening for diabetic retinopathy
- AI-assisted ophthalmic diagnosis
- Integration into telemedicine and public health systems
---

### 📚 Citation

If you use this repository or dataset, please cite the source dataset and Kaggle competition:

> APTOS 2019 Blindness Detection, Kaggle.  
> https://www.kaggle.com/datasets/sovitrath/diabetic-retinopathy-224x224-2019-data

---
### 🧑‍💻 Author

 Author : Houri razavi

 Email : hourirazavi@gmail.com
 
Project : Medical Image Classification – *Diabetic Retinopathy Detection*  

Focus: Deep learning for ophthalmic disease detection  

Field : AI in Healthcare / Medical Imaging
