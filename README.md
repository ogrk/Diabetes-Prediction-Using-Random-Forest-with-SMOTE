# 🩺 Diabetes Prediction using Random Forest with SMOTE

## 📖 Overview
This project predicts the likelihood of diabetes based on medical and lifestyle parameters using a **Random Forest Classifier** combined with **SMOTE** to address class imbalance.  
The workflow was developed entirely in **Google Colab**, and an instant web app version was deployed using **Replit** to demonstrate the model to faculty.

The model achieves:
- **Accuracy:** 96%
- **Precision (Class 1 - Diabetic):** 0.77
- **Recall (Class 1 - Diabetic):** 0.75
- **F1-Score (Class 1 - Diabetic):** 0.76

---

## 🔗 Model File (Google Drive Link)
Because the trained model file is too large to upload directly to GitHub, you can download it here:

👉 **Model Download:** *https://drive.google.com/file/d/1D2IZGUYNF9rjhhVQRGJ79jLkWo-ufTS0/view?usp=drive_link*

---

## 📊 Dataset
The dataset was sourced from **Kaggle**, containing the following features:

| Feature | Description |
|----------|--------------|
| `gender` | Male, Female, or Other |
| `age` | Age of the individual |
| `hypertension` | 0 = No, 1 = Yes |
| `heart_disease` | 0 = No, 1 = Yes |
| `smoking_history` | Current, Former, Never, etc. |
| `bmi` | Body Mass Index |
| `HbA1c_level` | Hemoglobin A1c level (%) |
| `blood_glucose_level` | Blood glucose level (mg/dL) |
| `diabetes` | Target variable (0 = Non-diabetic, 1 = Diabetic) |

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handled missing values  
- Converted categorical variables to numerical formats  
- Scaled numerical features where necessary  

### 2. Handling Class Imbalance
The dataset was imbalanced, with far fewer diabetic cases.  
To address this, we used **SMOTE (Synthetic Minority Oversampling Technique)** to generate synthetic minority samples.

### 3. Model Building
- Implemented a **Random Forest Classifier**
- Tuned key hyperparameters
- Trained in **Google Colab** for faster compute

### 4. Evaluation Metrics
We evaluated the model using:
- Precision
- Recall
- F1-score
- Accuracy

---

## 📈 Results

| Metric | Non-Diabetic (0) | Diabetic (1) |
|---------|------------------|--------------|
| Precision | 0.98 | 0.77 |
| Recall | 0.98 | 0.75 |
| F1-Score | 0.98 | 0.76 |

**Overall Accuracy:** 96%  
**Macro Avg F1:** 0.87  

---

## 🌐 Replit Instant Web App
We created a simple **web application on Replit** to display predictions to our professors during the project demonstration.

👉 The app allows users to input:  
- Age  
- BMI  
- HbA1c  
- Blood glucose level  
- Lifestyle factors  

And receive a real-time diabetes prediction using the trained Random Forest model.

You can adapt or clone the Replit code from this repo.

---

## 💡 Technologies Used
- Python
- Google Colab  
- pandas, numpy  
- scikit-learn  
- imbalanced-learn (SMOTE)  
- Replit (for instant web app deployment)  

---

## 🚀 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/diabetes-prediction-rf-smote.git
