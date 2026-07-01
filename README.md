
# Cyber Attack Detection Using PyTorch

## Overview

This project develops a deep learning-based system capable of detecting cyber attacks within network traffic. Using **PyTorch**, a neural network is trained to distinguish between normal and malicious network behavior. The system also supports **real-time anomaly detection**, helping improve network security by identifying suspicious activity.

---

## Features

- Neural network training using PyTorch  
- Cyber attack detection from network traffic data  
- Real-time anomaly detection support  
- Binary classification (Normal vs Attack)  
- Performance evaluation using accuracy metrics  

---

## Technologies Used

- Python 3.x  
- PyTorch  
- Pandas  
- NumPy  
- Scikit-learn  
- TorchMetrics  

---

## Project Structure


CyberAttackDetection/
│
├── data/
│ ├── labelled_train.csv
│ ├── labelled_test.csv
│ └── labelled_validation.csv
│
├── train.py
├── README.md
├── requirements.txt
└── .gitignore


---

## Dataset Setup (Important)

This project does not include large datasets. You must download and place them into the `data/` folder.

---

## Recommended Datasets

### CICIDS2017
:contentReference[oaicite:0]{index=0}  
Download: https://www.unb.ca/cic/datasets/ids-2017.html  

---

### NSL-KDD
:contentReference[oaicite:1]{index=1}  
Download: https://www.kaggle.com/datasets/hassan06/nslkdd  

---

### UNSW-NB15
:contentReference[oaicite:2]{index=2}  
Download: https://research.unsw.edu.au/projects/unsw-nb15-dataset  

---

## Required CSV Format

Your dataset must include a label column named:


sus_label


Example:


duration,protocol_type,src_bytes,dst_bytes,flag,sus_label


- `0` = Normal traffic  
- `1` = Attack / anomaly  

---

## Installation

```bash
git clone https://github.com/yourusername/CyberAttackDetection.git
cd CyberAttackDetection
pip install -r requirements.txt
Training the Model
python train.py
Testing the Model

The model evaluates:

Training accuracy
Validation accuracy
Test accuracy
Important Notes
Do NOT upload datasets to GitHub
Add this to .gitignore:
data/
Future Improvements
LSTM / Transformer-based detection
Real-time packet capture (Scapy / Wireshark integration)
REST API deployment
Live monitoring dashboard
Testing Workflow
Download dataset (CICIDS2017, NSL-KDD, or UNSW-NB15)
Place CSV files in data/
Run:
python train.py
View accuracy results
License

This project is for educational and research purposes.

Author

Cybersecurity + Machine Learning project using PyTorch for anomaly detection in network traffic.



## Author

Developed as a machine learning and cybersecurity project demonstrating deep learning techniques for network intrusion detection and real-time anomaly detection.
