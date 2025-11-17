# Hierarchical-Blockchain-Enabled-Secure-Aggregation-Algorithm-for-Federated-Learning-in-Heart-Disease

A cutting-edge, privacy-preserving Federated Learning (FL) framework enhanced with Hierarchical Blockchain, Secure Aggregation, and a Bayesian Time-Decayed Reputation System to build a trustworthy, attack-resilient, and scalable heart-disease prediction system.

This repository implements an advanced Federated Random Forest model secured by blockchain-anchored audit trails and dynamic reputation scoring — ensuring confidentiality, integrity, robustness, and high predictive accuracy.

🚀 Project Overview

Heart disease is one of the leading causes of death globally. Artificial Intelligence can assist clinicians in early diagnosis, but centralized ML pipelines require sensitive patient data to be moved to a central server, risking privacy, regulatory compliance, and security.

This project solves these challenges by introducing a secure, decentralized, blockchain-governed FL framework where:

✔ No patient data ever leaves the client/hospital

✔ Updates are validated through Proof-of-Quality (PoQ)

✔ Client behavior is monitored using Bayesian reputation scoring

✔ Only trustworthy updates are included in training

✔ Blockchain ensures transparency & tamper-proof audit trails

The result is a more accurate, robust, and reliable global model than centralized or traditional Federated Learning approaches.

🧬 Key Features
🔐 1. Privacy-Preserving Federated Learning

Local training on isolated hospital EHR datasets

Only model updates (not raw data) are shared

Random Forest classifier for interpretable risk prediction

🛡 2. Hierarchical Blockchain Layer

Sidechains for fast, low-latency interaction

Mainchain for anchoring global models & proofs

Merkle-root anchoring ensures integrity of each training round

Provides transparency, auditability, and tamper resistance

🧾 3. Proof-of-Quality (PoQ) Validation

Automatically filters poor, anomalous, or malicious model updates

Compares local validation metrics against round medians

Ensures only meaningful contributions enter the global model

⭐ 4. Bayesian Reputation Mechanism

Tracks long-term reliability of each participating hospital:

Time-decayed scoring

Penalizes unreliable or inconsistent updates

Rewards accurate and stable contributions

Only Top-K reputed clients participate in secure aggregation

📊 5. Reputation-Weighted Secure Aggregation

Prevents poisoning and low-quality update influence

Weighted averaging boosts overall performance

Enhances fairness, robustness, and security

📚 Datasets Used

This project uses two benchmark datasets widely used in cardiovascular risk prediction research.

1️⃣ Framingham Heart Study Dataset

✔ 4,240 patient records

✔ 16 columns / 15 clinical features

✔ Predicts 10-year risk of coronary heart disease (CHD)

Key features include:

Age

Gender

Systolic & Diastolic Blood Pressure

Total Cholesterol

Smoking Status

Diabetes

Heart Rate

Hypertension medication

Glucose levels

📌 Source: Kaggle (Aasheesh, 2023)

2️⃣ UCI Heart Disease Dataset

✔ 303 patient records

✔ 13 clinical features

✔ Binary classification (presence of heart disease)

Attributes include:

Age, sex

Chest pain type

Cholesterol

Resting ECG

Maximum heart rate

Exercise-induced angina

ST depression

🧼 Data Preprocessing Pipeline

To ensure data consistency across clients, each hospital performs:

✔ Missing value imputation

✔ Encoding of categorical attributes

✔ Standardization / normalization

✔ Stratified train-validation-test splits

70% Training

15% Validation

15% Testing

This guarantees balanced, fair evaluation across institutions.

🧠 System Architecture
Five Core Phases

Data Acquisition & Local Preprocessing

Feature Engineering & Local Model Training

Proof-of-Quality Validation & Reputation Update

Top-K Reputation-Based Secure Aggregation

Blockchain Anchoring & Global Model Deployment

🔗 Blockchain Architecture
Hierarchical Design

Sidechains:
Manage client interactions, PoQ validation, and reputation scoring.

Mainchain:
Stores cryptographic Merkle roots of aggregated global models.

Smart Contract-like Functionalities

Client registration

Update verification

Reputation posting

Penalty/reward allocation

Benefits

✔ Highly scalable

✔ Low latency

✔ Tamper-proof audit trails

✔ Trustless multi-party collaboration

🔎 Proposed Algorithms
Algorithm 1 — Federated Blockchain Heart Disease Prediction

Client registration

Local model training

Proof-of-Quality validation

Bayesian reputation update

Reputation-weighted aggregation

Blockchain anchoring

Algorithm 2 — Secure Aggregation

Select Top-K reputed clients

Merge model updates using reputation-based weights

Anchor Merkle root in mainchain for tamper-proof recording

📈 Results
Performance Comparison
Method	Accuracy	Precision	Recall	F1-Score
Centralized RF	86.7%	0.87	0.85	0.86
Federated RF (No Blockchain)	84.5%	0.85	0.82	0.83
Proposed HB-FL + Reputation	89.8%	0.90	0.88	0.89
Highlights

🚀 Outperforms centralized & plain FL models

🛡 Highly resistant to poisoning attacks

📉 Stable accuracy even with malicious clients

🎯 Optimal reputation threshold ≈ 0.45

🔝 Top-12 reputed clients give best performance

🛠️ Tech Stack

Python

Scikit-Learn

NumPy / Pandas

Matplotlib / Seaborn

Custom Blockchain Simulation Layer

Federated Learning Orchestration Engine

🔮 Future Enhancements

Integration with Hyperledger Fabric / Ethereum POA chains

Deployment on real healthcare IoT sensors

Add Differential Privacy (DP) to prevent gradient leakage

Support for deep neural networks in federated settings

Reinforcement Learning-based adaptive client selection

Real-time FL monitoring dashboards
