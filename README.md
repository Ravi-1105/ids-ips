# ids-ips

# 🔐 Basic Intrusion Detection System (IDS) using Machine Learning

This project is a simple yet powerful Intrusion Detection System built using Python and machine learning. It uses a labeled dataset (e.g., CICIDS2017 or similar) to detect whether a network traffic flow is **BENIGN** or an **ATTACK**.

---

## 📁 Dataset

- The dataset should be a CSV file with network traffic features and a final column named `Label`.
- Example: CICIDS2017 or a sample subset with features like `Flow Duration`, `Total Fwd Packets`, `Bwd Packet Length Max`, etc.

You can download the full dataset here:  
➡️ [https://www.unb.ca/cic/datasets/ids-2017.html](https://www.unb.ca/cic/datasets/ids-2017.html)

---

## 🧰 Tech Stack

- **Language**: Python 3.x  
- **Libraries**: 
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`

---
## Project Structure
```
IDS-ML/
├── cicids_sample.csv              # Input dataset file
├── ids_detection_cicids.py        # Main detection script
├── README.md                      # Project documentation
└── requirements.txt               # Python dependencies

```
## 🚀 How It Works

1. Preprocess the dataset:
   - Handle missing values
   - Scale numerical features
   - Encode the `Label` column: `BENIGN` = 0, `ATTACK` = 1

2. Train/Test split using `train_test_split`

3. Train a Random Forest classifier on the training data

4. Evaluate the classifier using accuracy, precision, recall, F1-score, and a confusion matrix

---

## 📌 Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/Basic-IDS-ML.git
cd Basic-IDS-ML
```
### Install Dependencies
```bash
pip install -r requirements.txt
```
## Output:
![ids-op](https://github.com/user-attachments/assets/34507f3f-a7aa-4c4e-8708-4734ed77a086)
