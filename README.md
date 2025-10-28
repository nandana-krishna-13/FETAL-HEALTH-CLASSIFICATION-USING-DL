# 🩺 Fetal Health Classification Using Deep Learning Models on Cardiotocography (CTG) Data  

## 📘 Overview  
This project aims to automate fetal health classification using Deep Learning (DL) models applied to Cardiotocography (CTG) data, which records **Fetal Heart Rate (FHR)** and **Uterine Contractions (UC)**.  
Manual CTG interpretation is time-consuming and prone to human error. This study leverages DL models to improve **accuracy, speed, and reliability** in fetal health analysis — ultimately helping reduce fetal health risks.

---

## 🎯 Objectives  
- Automate fetal health classification using CTG data.  
- Compare performance across multiple DL architectures.  
- Identify abnormal fetal patterns to aid timely clinical interventions.

---

## 📊 Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/) & [Kaggle](https://www.kaggle.com/datasets/propanon/uci-cardiotocography)  
- **Samples:** 2,126 fetal cardiotocograms  
- **Features:** 33 (including FHR, UC, and variability measures)  
- **Labels:**  
  - **Fetal States:** Normal (N), Suspect (S), Pathologic (P)  
  - **Morphologic Patterns:** 10 CTG waveform classes  

---

## 🧠 Models Implemented  
1. **Shallow LSTM** – Two-layer architecture capturing temporal dependencies.  
2. **Deep LSTM** – Three-layer model for complex sequential patterns.  
3. **CNN (1D)** – Extracts local temporal features from CTG signals.  
4. **FNN** – Feedforward Neural Network capturing non-sequential relationships.  

All models were trained using the **Adam optimizer** and **Sparse Categorical Cross-Entropy** loss.

---

## 📈 Results & Analysis  

| Model | Validation Accuracy | Observations |
|--------|----------------------|---------------|
| **Deep LSTM** | ⭐ Highest | Most stable and accurate model |
| **Shallow LSTM** | High | Balanced performance |
| **CNN** | Moderate | Risk of overfitting |
| **FNN** | Low | Poor convergence |

**Conclusion:** LSTM-based models outperform others in capturing CTG’s sequential nature.

---

## 📊 Visualization  
Comparative plots include:  
- Accuracy and Loss Curves  
- ROC and AUC Curves across models  

> Deep LSTM achieved an **AUC of 0.99**, indicating strong classification reliability.

---

## 🧾 Notebook
📓 **Main Notebook:** [DL_Project_Group_10.ipynb](DL_Project_Group_10.ipynb)


## 🧾 Links  
- 📘 **Colab Notebook:** [View Here](https://colab.research.google.com/drive/1MSPYHMVsgyauyEFUHLlCmLd2CL6ktqIw?usp=sharing)  
- 📊 **Dataset:** [Kaggle Dataset](https://www.kaggle.com/datasets/propanon/uci-cardiotocography)

---

## 🧰 Technologies Used  
- Python  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib  
- Google Colab  
