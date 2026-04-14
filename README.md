# AI-Based-Early-Sepsis-Prediction-System
Machine learning system for early sepsis prediction using ICU patient data
📌 Overview
This project focuses on early prediction of sepsis using machine learning techniques on real ICU patient data.  
The system analyzes vital signs and predicts whether a patient is at risk, enabling early intervention in healthcare settings.

 🎯 Problem Statement
Traditional monitoring systems rely on fixed thresholds and often fail to detect early signs of deterioration.  
This project aims to build an intelligent system that predicts sepsis risk using patient data.

📊 Dataset
- Source: PhysioNet (2019 Sepsis Challenge Dataset)
- Type: ICU patient time-series data
- Each file represents one patient with multiple time-based observations

 ⚙️ Methodology
 🔹 Data Processing
- Combined multiple patient files into a single dataset  
- Handled missing values using forward-fill, backward-fill, and median imputation  
- Converted time-series data into **patient-level aggregated data**
 🔹 Feature Engineering
- Pulse Pressure = SBP - DBP  
- Shock Index = HR / SBP
   🔹 Handling Imbalance
- Applied **SMOTE** to balance the dataset
 🔹 Model Training
- Logistic Regression  
- Random Forest  
- XGBoost  
 🔹 Model Selection
- Evaluated using Accuracy, Precision, Recall, F1-score, ROC-AUC  
- Selected **XGBoost** as final model  

 📈 Results
- Final Model: XGBoost  
- ROC-AUC: **0.85**  
- Improved detection of high-risk sepsis patients  
- Balanced performance using optimized threshold (0.4)

 🧠 Key Features
- Early risk prediction of sepsis  
- Uses real-world ICU data  
- Feature engineering based on clinical indicators  
- Handles class imbalance effectively  
- Designed for real-time healthcare applications  

 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn
