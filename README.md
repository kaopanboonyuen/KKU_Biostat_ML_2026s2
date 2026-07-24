# 🧠 Fundamental Machine Learning using Python for Public Health
### A Two-Day Hands-on Workshop

> **Machine Learning for Public Health**
> Department of Biostatistics
> Faculty of Public Health, Khon Kaen University
> Semester 2, Academic Year 2026

<p align="center">

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![MIT](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

</p>

---

## 📖 Overview

This repository contains the official teaching materials for the two-day workshop **Fundamental Machine Learning using Python for Public Health**, designed for graduate students in the **Master of Public Health (Biostatistics)** program, Faculty of Public Health, Khon Kaen University.

Participants work hands-on with a real clinical stroke-prediction dataset, moving from Python fundamentals all the way to PyTorch neural networks — the complete modern ML workflow for healthcare applications.

## 👨‍🏫 Lecturer

**Dr. Teerapong Panboonyuen (Kao)** — AI Researcher • Computer Vision • Medical AI • Machine Learning
[kaopanboonyuen.github.io](https://kaopanboonyuen.github.io/)

## 🎯 Learning Outcomes

- Prepare and explore real-world healthcare datasets with `pandas`
- Engineer clinically meaningful features from raw patient data
- Build and evaluate supervised ML models: Decision Trees, Random Forests, Logistic Regression
- Handle missing values and imbalanced clinical outcomes correctly
- Understand neural networks from first principles, and build them in **PyTorch**
- Compare classical ML vs. Deep Learning fairly, using the right metrics
- Apply reproducible, ethical AI research practices in public health

---

## 🗓️ Workshop Schedule

### 📅 Day 1 — Python Foundations, Feature Engineering & Your First ML Models

> 🎯 **Goal**: Refresh core Python for data science, explore a real stroke-risk dataset, engineer clinically meaningful features, and train + evaluate your first classifiers.

#### 🛠️ Lab Activity: KKU Stroke Dataset

| Resource | Link |
|:---|:---|
| 🧠 Lecture Slide | [Day1_KKU_Biostat_ML.pdf](https://github.com/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/slides/Day1_KKU_Biostat_ML.pdf) |
| 🧪 Colab Notebook | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/code/Day1_KKU_Biostat_ML.ipynb) |
| 📂 Dataset | [kku-stroke-dataset.csv](https://github.com/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/dataset/kku-stroke-dataset.csv) |

> 💡 **Lab Topics**
>
> - Python refresher: variables, operators, conditionals, loops, containers, functions, classes
> - Loading and exploring the dataset with `pandas`: missingness, class imbalance, rich EDA
> - Feature engineering: clinical binning (WHO BMI / ADA glucose), encoding, composite risk scores
> - Building a supervised learning pipeline: stratified split → Decision Tree → Random Forest
> - Feature importance, and full evaluation: Accuracy, Precision, Recall, F1, ROC-AUC, confusion matrix

<details>
<summary>📖 Dataset Dictionary — KKU Stroke Dataset</summary>

| Column | Description |
|:---|:---|
| `id` | Unique participant identifier |
| `gender` | Male / Female / Other |
| `age` | Age in years |
| `hypertension` | History of hypertension (0 = No, 1 = Yes) |
| `heart_disease` | History of heart disease (0 = No, 1 = Yes) |
| `ever_married` | Marital status (Yes/No) |
| `work_type` | Private, Self-employed, Govt_job, children, Never_worked |
| `Residence_type` | Urban / Rural |
| `avg_glucose_level` | Average blood glucose level (mg/dL) |
| `bmi` | Body Mass Index (kg/m²) — contains missing values |
| `smoking_status` | never smoked / formerly smoked / smokes / Unknown |
| `stroke` | **Target** — Stroke diagnosis (0 = No, 1 = Yes) |

</details>

---

### 📅 Day 2 — Logistic Regression, Neural Networks & Deep Learning

> 🎯 **Goal**: Understand Logistic Regression and neural networks from first principles, build real PyTorch models (including a 1D CNN), and close with a guide to responsible AI research in public health.

#### 🛠️ Lab Activity: Stroke Risk Modeling — Classical ML vs. Deep Learning

| Resource | Link |
|:---|:---|
| 🧠 Lecture Slide | [Day2_KKU_Biostat_ML.pdf](https://github.com/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/slides/Day2_KKU_Biostat_ML.pdf) |
| 🧪 Colab Notebook | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/code/Day2_KKU_Biostat_ML.ipynb) |
| 📂 Dataset | [kku-stroke-dataset.csv](https://github.com/kaopanboonyuen/KKU_Biostat_ML_2026s2/blob/main/dataset/kku-stroke-dataset.csv) |

> 💡 **Lab Topics**
>
> - Logistic Regression from first principles: sigmoid, logit, binary cross-entropy, gradient descent
> - The bridge from a single neuron to full neural networks
> - Hands-on **PyTorch**: a Simple MLP, a Deeper MLP (Dropout + BatchNorm), and a 1D CNN for automatic feature learning
> - Reading a paper's Methods section: epochs, learning rate, batch size, optimizer, regularization
> - Fair model comparison — Decision Tree / Random Forest / Logistic Regression / Neural Nets — same data, same metrics
> - Reproducible research practices and responsible/ethical AI use in public health

---

## 🏥 Hands-on Dataset

The **KKU Stroke Dataset** is a real-world healthcare dataset (credit: [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)) with demographic, clinical, and lifestyle features for predicting stroke risk.

- **Task:** Binary classification — Target variable: `stroke`
- **Challenges:** Missing values, class imbalance, mixed numerical/categorical variables, clinical interpretability

## 🛠 Software Stack

| Category | Libraries |
|---|---|
| Programming | Python 3.11 |
| Data Analysis | NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| Classical ML | Scikit-learn |
| Deep Learning | PyTorch |
| Environment | Jupyter Notebook / Google Colab |

## 📚 Reference

Melnykova, N., et al. (2025). **Machine learning for stroke prediction using imbalanced data.** *Scientific Reports*, 15(1), 33773.

## 📖 Citation

```bibtex
@misc{Panboonyuen2026ML4PH,
  author       = {Teerapong Panboonyuen},
  title        = {Fundamental Machine Learning using Python for Public Health},
  year         = {2026},
  publisher    = {GitHub},
  howpublished = {https://github.com/kaopanboonyuen/KKU_Biostat_ML_2026s2},
  note         = {Lecture for the Master of Public Health (Biostatistics) Program, Department of Biostatistics, Faculty of Public Health, Khon Kaen University}
}
```

## 🤝 Acknowledgements

Organized for the Master of Public Health (Biostatistics) program, Faculty of Public Health, Khon Kaen University. Dataset credit: Kaggle. Built with scikit-learn and PyTorch. Thanks to all students for their enthusiasm throughout the workshop.

## 📜 License

Released under the **MIT License**. Intended primarily for educational and research purposes — please provide attribution when reusing substantial portions of this repository.

---

<p align="center">

*"From healthcare data to scientific discovery through reproducible machine learning."*

</p>