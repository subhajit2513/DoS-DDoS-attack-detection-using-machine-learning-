# DoS-DDoS-attack-detection-using-machine-learning-
# 🚨 DoS/DDoS Attack Detection Using Machine Learning

**Internship Project at NIELIT Kolkata**  
**Department of Computer Science and Technology (MCA)**  
**Jadavapur University, 2025**

A collaborative research project aimed at detecting Denial-of-Service (DoS) and Distributed Denial-of-Service (DDoS) attacks using machine learning and deep learning models on real-world network traffic datasets. The system integrates traditional ML models, transformer-based deep learning, and real-time packet analysis using tools like Wireshark and the Elastic Stack.

---

## 🧠 Project Overview

DoS/DDoS attacks are among the most disruptive cyber threats, targeting network availability through resource exhaustion. Traditional firewalls and signature-based IDS often fail to detect novel attack patterns. This project proposes a hybrid, intelligent detection system using supervised ML classifiers, real-time traffic monitoring, and deep contextual analysis to identify malicious patterns with high accuracy.

> 📊 **Best Performing Model: BERT-inspired Transformer — 97.1% Accuracy**

---

## 🔍 Objectives

- Detect DoS/DDoS patterns using packet-level features and protocol behaviors.
- Train multiple ML models (SVM, Random Forest, Logistic Regression, etc.)
- Apply advanced deep learning (BERT/Transformer, LSTM) for contextual analysis.
- Use Wireshark for real-time traffic capture.
- Visualize live traffic insights using the ELK Stack (Elasticsearch, Logstash, Kibana).
- Ensure detection scalability and interpretability via SHAP and attention scores.

---

## 📁 Dataset

- **CICIDS 2017**, **UNSW-NB15**, and **NSL-KDD** datasets.
- Preprocessed `.csv` files labeled for binary classification (attack vs. normal).
- Includes SYN flood, UDP flood, Slowloris, ICMP flood, HTTP GET floods.
- **Dataset Used**: [CICIDS 2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html)
- **Description**: Includes realistic network traffic labeled with different attack types including DoS and DDoS attacks.

---

## ⚙️ Technologies Used

| Category            | Tools & Libraries                                   |
|---------------------|-----------------------------------------------------|
| Language            | Python                                               |
| ML Libraries        | scikit-learn, pandas, NumPy                         |
| Deep Learning       | PyTorch, HuggingFace Transformers                   |
| Visualization       | Matplotlib, Seaborn, Kibana                         |
| Packet Sniffing     | Wireshark, Scapy, PyShark                           |
| Web Interface       | Flask, React (for simulation and dashboard)         |
| Hosting             | GitHub, Render.com                                  |

---

## 🧪 Models Implemented

| Model                  | Accuracy | Notes                                    |
|------------------------|----------|------------------------------------------|
| Random Forest          | 98.5%    | High F1-score, robust to overfitting     |
| Support Vector Machine | 94.5%    | Great for high-dimensional classification|
| Logistic Regression    | 92.8%    | Fast, interpretable                      |
| Naive Bayes            | 90.2%    | Lightweight, baseline comparison         |
| BERT/Transformer       | 97.1%    | Best contextual detection performance    |

---

## 📊 Evaluation Metrics

- Accuracy, Precision, Recall, F1-Score
- Confusion Matrix
- ROC-AUC
- SHAP for explainability (in tree models)
- Attention Visualization (for transformer models)

---

+--------------------+
| Packet Capture     |
| (tcpdump / Zeek)   |
+--------------------+
          ↓
+--------------------+
| Flow Generator     |
| (Zeek / CICFlow)   |
+--------------------+
          ↓
+--------------------+
| Feature Engineering|
| (Python / Pandas)  |
+--------------------+
          ↓
+--------------------+
| ML Inference       |
| (RF / SVM)         |
+--------------------+
          ↓
+--------------------+
| Alerting & Dashboards |
| (ELK + Flask API)  |
+--------------------+

# Created_By
KUNAL DHIBAR & SUBHAJIT DAS
---



