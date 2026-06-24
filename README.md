# Diabetes Risk Prediction Using Classical Machine Learning and Deep Learning

**Advancing Preventive Healthcare in Rwanda and Africa**

## 📋 Project Overview

This project presents a comprehensive, end-to-end comparative study of **classical machine learning** and **deep learning** approaches for early **diabetes risk prediction**. Developed as an academic assignment and personal mission-driven initiative, it addresses the growing diabetes burden in Rwanda and Sub-Saharan Africa through accurate, deployable predictive models.

The pipeline systematically progresses through eight experiments — from a baseline Random Forest to a highly stabilized deep neural network (Experiment 8) — incorporating best practices in preprocessing, regularization, class imbalance handling (Focal Loss), learning rate scheduling, and thorough evaluation.

**Best Model**: **Experiment 8** — Stabilized Focal Neural Network  
**Key Metrics (Validation)**: Accuracy 0.9733 | Precision **1.0000** | Recall 0.6863 | F1 0.8140 | **ROC-AUC 0.9789**

The models are designed to power mobile screening tools, community health worker apps, and clinical decision support systems, while creating technology-driven employment opportunities for youth in Rwanda and Africa.

---

## ✨ Key Features

- **Comparative Analysis**: Classical ML (Random Forest variants) vs. Deep Learning (Sequential & Functional APIs)
- **Robust Preprocessing**: Standardization, one-hot encoding, stratified splitting, and optimized `tf.data` pipelines
- **Advanced Techniques**:
  - Hyperparameter tuning with GridSearchCV
  - Feature importance and class weighting
  - Dropout, L2 regularization, Batch Normalization
  - Focal Loss for class imbalance
  - Cosine decay + ReduceLROnPlateau scheduling
  - EarlyStopping and ModelCheckpoint
- **Comprehensive Evaluation**: Accuracy, Precision, Recall, F1, ROC-AUC, confusion matrices, and learning curves
- **Reproducibility**: Fixed random seeds and detailed documentation
- **Clinical Focus**: Emphasis on high precision (zero false positives in Exp8) and meaningful recall for real-world screening

---

## 📊 Dataset

- **Source**: [Diabetes Prediction Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset) on Kaggle
- **Size**: ~100,000 records
- **Features**: Age, BMI, HbA1c level, blood glucose, hypertension, heart disease, smoking history, gender, etc.
- **Target**: Binary diabetes diagnosis (imbalanced dataset)

---

## 🛠️ Technologies Used

- **Python** 3.10+
- **Data Science**: pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn (Random Forest, GridSearchCV)
- **Deep Learning**: TensorFlow / Keras (Sequential, Functional API, tf.data)
- **Utilities**: Joblib, warnings suppression, reproducibility seeds

---

## 🚀 How to Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/diabetes-risk-prediction.git
   cd diabetes-risk-prediction
   ```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow joblib
```

3. Download the dataset:

- Place **diabetes_prediction_dataset.csv in the project root**

4. Open the notebook:
```bash
jupyter notebook "Diabetes Risk Prediction.ipynb"
```

5. Run cells sequentially. All random seeds are fixed for full reproducibility.

**Note** : Training deep learning models may require a GPU for faster execution, but the notebook runs comfortably on CPU.

## 🌍 Mission & Impact

- This project is more than a technical exercise. It is aligned with a broader vision of using AI to create sustainable employment for youth in Rwanda and Africa by 2035. The developed system opens opportunities in health data collection, model monitoring, mobile app development, telemedicine, and local healthtech entrepreneurship.

- By enabling early diabetes detection, the models can reduce complications, lower healthcare costs, and support community-level preventive programs across the continent.

## 🔮 Future Work

- Advanced oversampling (SMOTE/ADASYN) to improve recall
- Hybrid RF + Neural Network ensembles
- Integration of Rwanda/Africa-specific features (diet, genetics, socioeconomic data)
- Deployment as a lightweight mobile/web application
- Continuous retraining pipeline with community-collected data

## 📜 License

This project is open for educational and research purposes. Feel free to use, modify, and build upon it. Please provide appropriate credit.

## 👤 Author

**Francis Mutabazi**
Aspiring AI Engineer & Healthtech Advocate
Passionate about leveraging technology for preventive healthcare and youth empowerment in Africa.
