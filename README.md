# 🩺 Diabetes Prediction using Random Forest with SMOTE

## 📖 Overview
This project aims to predict whether an individual is diabetic or not based on various medical and lifestyle parameters.  
We used the **Random Forest** algorithm combined with **SMOTE (Synthetic Minority Over-sampling Technique)** to effectively handle class imbalance in the dataset.

The model achieves:
- **Accuracy:** 96%
- **Precision (Class 1 - Diabetic):** 0.77  
- **Recall (Class 1 - Diabetic):** 0.75  
- **F1-Score (Class 1 - Diabetic):** 0.76  

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
| `diabetes` | Target variable (0 = No, 1 = Yes) |

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Cleaned missing values
   - Encoded categorical variables (e.g., gender, smoking history)
   - Normalized/standardized numerical features

2. **Handling Imbalance**
   - Used **SMOTE** (Synthetic Minority Oversampling Technique) to balance diabetic and non-diabetic classes.

3. **Model Building**
   - Implemented **Random Forest Classifier**
   - Tuned hyperparameters for best performance

4. **Evaluation Metrics**
   - Accuracy, Precision, Recall, and F1-score

---

## 📈 Results
| Metric | Non-Diabetic (0) | Diabetic (1) |
|---------|------------------|--------------|
| Precision | 0.98 | 0.77 |
| Recall | 0.98 | 0.75 |
| F1-Score | 0.98 | 0.76 |

**Overall Accuracy:** 96%  
**Macro Avg F1-Score:** 0.87  

These results indicate that the model performs extremely well overall, with strong predictive power for the diabetic class after applying SMOTE.

---

## 💡 Technologies Used
- Python 🐍
- pandas, numpy
- scikit-learn
- imbalanced-learn (for SMOTE)
- matplotlib / seaborn (for visualization)
- Jupyter Notebook / Google Colab

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/diabetes-prediction-rf-smote.git
