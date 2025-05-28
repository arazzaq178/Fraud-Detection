## 🕵️‍♂️ Fraud Detection System Using Machine Learning

This project is a complete implementation of a fraud detection system using the [Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud). The system applies machine learning to detect fraudulent credit card transactions, using **Random Forest Classifier** and handling class imbalance with **SMOTE**.

---

### 📁 Project Structure

```
fraud_detection/
│
├── creditcard.csv           # Dataset file (not included due to size)
├── fraud_model.pkl          # Trained model (auto-generated after training)
├── fraud_detection.ipynb    # Jupyter Notebook with step-by-step code
├── fraud_detection.py       # Python script version (optional)
└── README.md                # This file
```

---

### 🚀 Features

* Data Preprocessing

  * Converts float columns to integers
  * Handles class imbalance using SMOTE
* Model Training with Random Forest
* Evaluation using Precision, Recall, and F1-Score
* CLI testing interface to check if a transaction is fraudulent or not
* Model saving and loading using `joblib`

---

### 🛠️ Installation

1. Clone the repository or download the code:

   ```bash
   git clone https://github.com/yourusername/fraud-detection.git
   cd fraud-detection
   ```

2. Install required libraries:

   ```bash
   pip install pandas numpy scikit-learn imbalanced-learn joblib
   ```

---

### 📊 How to Run

#### Option 1: In Jupyter Notebook (Recommended)

* Open `fraud_detection.ipynb`
* Run all cells **manually** step-by-step for:

  * Loading and preprocessing data
  * Training and evaluating model
  * Testing custom input

#### Option 2: As Python Script

* Make sure `creditcard.csv` is in the correct folder
* Run the script:

  ```bash
  python fraud_detection.py
  ```

---

### 🎯 Testing the Model

Once trained, you can test the model by entering 30 transaction features as comma-separated values.

Example input:

```
-1.35980713, -0.072781173, 2.53634674, 1.37815522, ..., 0.0
```

---

### 📈 Evaluation Metrics

After training, the model prints a classification report including:

* Precision
* Recall
* F1-Score

These metrics help measure how well the model detects fraud without flagging legitimate transactions.

---

### 📌 Requirements

* Python 3.7+
* pandas
* numpy
* scikit-learn
* imbalanced-learn (`SMOTE`)
* joblib

---

### 📚 Dataset Source

> [Credit Card Fraud Detection Dataset - Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

---

### 📦 Future Improvements

* Use Gradient Boosting or XGBoost for higher accuracy
* Deploy as a Flask or FastAPI web service
* Integrate real-time streaming input
