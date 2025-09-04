# Multistage-Intrusionn-Detection-System-for-Adversarial-Attacks-based-on-Ensemble-model-in-IoT
ML-based IDS (Intrusion Detection System) for IoT. Tested against adversarial attacks to improve robustness and security.
This project focuses on building a robust Intrusion Detection System (IDS) for IoT environments, capable of detecting cyberattacks and resisting Adversarial Machine Learning (AML) attacks. By combining hybrid ensemble models with adversarial training, the system enhances security in IoT-based smart cities.
Dataset
Source: DS2OS (Distributed Smart Space Orchestration System) dataset
Size: ~3.58 lakh samples (3,47,935 normal + 10,027 attack samples)
IoT Devices Simulated: light controllers, thermostats, solar batteries, door locks, washing machines, smartphones, movement sensors

Attack Scenarios (7):
Net Scan
Spying
Malicious Control
Malicious Operation
DoS
Data Probing
Wrong Setup

Features: 13 attributes (e.g., source/destination ID, location, operation, timestamp, etc.)

Methodology
Data Preprocessing
Missing value imputation
Label encoding for categorical variables
Standardization for numerical features
Feature Engineering
Extraction of correlation-based features
Selection of top 5 features for training
Hybrid Models
RDL: Random Forest + Deep Neural Network + Logistic Regression
RDS: Random Forest + Deep Neural Network + Support Vector Machine
Adversarial Attack Simulation
FGSM, JSMA, BIM, PGD, DeepFool
Robust Training
Generated adversarial samples from test data
Augmented dataset with adversarial + clean data
Retrained models for resilience
Evaluation Metrics
Accuracy, Precision, Recall, F1-score
Confusion Matrix, ROC curves

Results
Baseline Accuracy: ~99%
Under Adversarial Attacks: ~98%
Enhanced Detection: Strong resilience against multi-stage & anomaly-based attacks

Key Insight: Retraining with adversarial samples significantly improves IDS robustness.

Technologies Used

Languages & Libraries:
Python
Scikit-learn
TensorFlow / Keras
Pandas, NumPy
Matplotlib, Seaborn 
Platform: Google Colab

Key Features
Robust IDS for IoT smart cities
Handles adversarial attacks effectively
Hybrid ensemble approach (classical + deep learning models)
Supports multi-stage and anomaly-based detection
