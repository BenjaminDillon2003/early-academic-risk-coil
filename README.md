# 🎓 Early Academic Risk Prediction (COIL Project)

This repository contains the full implementation of our AI model for predicting *early academic risk* in students using logistic regression.  
The project was developed collaboratively between **Universidad San Francisco de Quito (USFQ)** and **Virginia Tech (VT)** as part of the *COIL – Collaborative Online International Learning* initiative.

---

## 🚀 Project Overview

The goal of this project is to build a machine learning model capable of identifying students at risk (Low, Medium, High) based on performance indicators.  

We use:  
- A **real dataset** from Kaggle (`Students Performance`)  
- A **synthetic labeled dataset** generated using Python  
- A full preprocessing + model training pipeline  
- Logistic Regression  
- Colab demo notebook  
- A fully documented repository structure  

---

## 📂 Repository Structure
early-academic-risk-coil/
│
├── code/ # All source code (Python)
│ └── model_pipeline.py
│
├── data/ # Input datasets
│ ├── StudentsPerformance.csv
│ └── synthetic_dataset.csv
│
├── report/ # Final written report
│ └── Early_Academic_Risk_Report.pdf
│
└── README.md # Project description (this file)


---

## 📊 Dataset & Labels

### **Dataset 1 — Kaggle (Real Data)**  
Source: *Students Performance* dataset  
Features used:
- Math score  
- Reading score  
- Writing score  
- Gender  
- Lunch  
- Parental education  
- Test preparation  

### **Dataset 2 — Synthetic Dataset (Our Labels)**  
We generated a three-class label:

| Label | Meaning     |
|-------|-------------|
| 0     | Low Risk    |
| 1     | Medium Risk |
| 2     | High Risk   |

Label rules were created based on weighted score averages.

---

## 🧠 Machine Learning Model

We use **Logistic Regression (multi-class)** from Scikit-Learn.

Pipeline:
1. Load dataset  
2. Encode categorical features  
3. Train/Test split  
4. Train Logistic Regression (max_iter=2000)  
5. Evaluate: accuracy, precision, recall, F1  
6. Display confusion matrix  

Typical performance:
Accuracy: 0.74
Macro Avg F1: 0.73


---

## 📹 Demo Video (Insert Link)
https://drive.google.com/file/d/1Da8R82eLFrU8gIX9x7jry3FdpA8LPixv/view?usp=sharing


The video includes:  
- Project motivation  
- Dataset explanation  
- Labeling method  
- Model pipeline walkthrough  
- Live Google Colab demo  
- Discussion of ethical concerns  

---

## ▶️ Running the Model (Google Colab)

No manual downloads required.  
The script pulls datasets directly from GitHub.

### **1. Open the notebook**
https://colab.research.google.com/drive/15w-HJUPiMESoted5yn4F9Ahv4JfY5PL0?usp=sharing


### **2. Install dependencies**
```python
pip install pandas scikit-learn matplotlib seaborn

3. Run all cells

The notebook automatically:

Loads the datasets

Processes the data

Trains the model

Shows accuracy

Displays confusion matrix


Authors
Benjamín Dillon Gangotena – Universidad San Francisco de Quito

Full model pipeline

Data preprocessing

Synthetic label generation

Google Colab demo

Repo organization

Final report & presentation

Ayman Sharieff – Virginia Tech

Dataset research

Feature analysis

Risk labeling criteria

Presentation development

Ethical framework

Technologies Used

Python 3

Scikit-Learn

Pandas

Seaborn

Matplotlib

Google Colab

Git + GitHub


