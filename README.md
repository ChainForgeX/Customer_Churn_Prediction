# 🧠 Customer Churn Prediction using Deep Learning

**An end-to-end Deep Learning project predicting bank customer churn using an Artificial Neural Network built with TensorFlow and Keras**

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)](https://keras.io/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

[![Dataset](https://img.shields.io/badge/Dataset-Churn_Modelling-blue?style=flat)](#-dataset)
[![Model](https://img.shields.io/badge/Model-ANN-orange?style=flat)](#-model-architecture)
[![Task](https://img.shields.io/badge/Task-Binary_Classification-green?style=flat)](#-dataset)
[![License](https://img.shields.io/badge/License-MIT-brightgreen?style=flat)](#-license)

> **Complete supervised Deep Learning lifecycle — data preprocessing, encoding, feature scaling, ANN design, training, evaluation, and model persistence.**

---

## 📑 Table of Contents

- [Overview](#-project-overview)
- [Features](#-features)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Model Pipeline](#-model-pipeline)
- [Data Preprocessing](#️-data-preprocessing)
- [Model Architecture](#-model-architecture)
- [Workflow](#️-workflow)
- [Evaluation Metrics](#-evaluation-metrics)
- [Tech Stack](#️-tech-stack)
- [Getting Started](#-getting-started)
- [Screenshots](#-screenshots)
- [Skills Demonstrated](#-skills-demonstrated)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 📖 Project Overview

Customer churn is one of the biggest challenges in the banking industry — retaining existing customers is often far more cost-effective than acquiring new ones. This project uses an **Artificial Neural Network (ANN)** built with TensorFlow and Keras to analyze customer demographic and financial information and predict the probability that a customer will leave the bank.

The project follows a professional supervised Deep Learning workflow: data cleaning, label and one-hot encoding, feature scaling, ANN design and training, performance evaluation, and model persistence.

---

## 📌 Features

- Customer Churn Prediction using Artificial Neural Networks
- Complete Data Preprocessing Pipeline
- Label Encoding & One-Hot Encoding
- Feature Scaling using StandardScaler
- TensorFlow Sequential Neural Network
- Binary Classification using Sigmoid Activation
- Model Evaluation with Accuracy, Confusion Matrix & Classification Report
- Model Saving & Loading
- Clean and Modular Code Structure

---

## 📊 Dataset

**Dataset:** Churn Modelling Dataset
**Source:** Kaggle

### Dataset Statistics

| Property        | Value                |
| ---------------- | --------------------- |
| Features          | 11                    |
| Target             | `Exited`              |
| Learning Type   | Supervised Learning   |
| Task                | Binary Classification |

### Feature Descriptions

| Feature             | Description                                |
| -------------------- | ------------------------------------------- |
| `CreditScore`      | Customer's credit score                     |
| `Geography`         | Customer's country of residence             |
| `Gender`             | Customer gender                             |
| `Age`                  | Customer age                                |
| `Tenure`             | Number of years as a bank customer          |
| `Balance`            | Account balance                             |
| `NumOfProducts`   | Number of bank products used                |
| `HasCrCard`         | Whether the customer has a credit card      |
| `IsActiveMember` | Whether the customer is an active member    |
| `EstimatedSalary` | Customer's estimated salary                 |

### Target Variable

`Exited`

- `0` → Customer Stayed
- `1` → Customer Left

---

## 📂 Project Structure

```
Customer_Churn_Prediction/
│
├── data/
│   └── Churn_Modelling.csv
│
├── notebooks/
│   └── Customer_Churn_Prediction.ipynb
│
├── models/
│   └── churn_model.keras
│
├── images/
│   ├── confusion_matrix.png
│   ├── epoch_vs_accuracy.png
│   ├── epoch_vs_loss.png
│   └── exited.png
│
├── requirement.txt
├── .gitignore
└── README.md
```

---

## 🔄 Model Pipeline

```
flowchart TD
    A[📦 Import Dataset] --> B[🔍 Exploratory Data Analysis]
    B --> C[🧹 Data Cleaning]
    C --> D[🔤 Label Encoding]
    D --> E[🔢 One-Hot Encoding]
    E --> F[✂️ Train-Test Split]
    F --> G[⚙️ Feature Scaling\nStandardScaler]
    G --> H[🤖 Build ANN with TensorFlow]
    H --> I[🛠️ Compile Model]
    I --> J[🏋️ Train Model]
    J --> K[📏 Evaluate Performance]
    K --> L[🎯 Generate Predictions]
    L --> M[💾 Save Trained Model]
```

---

## ⚙️ Data Preprocessing

| Step                    | Technique                                   |
| ------------------------ | -------------------------------------------- |
| Categorical Encoding | Label Encoding & One-Hot Encoding           |
| Feature Scaling        | `StandardScaler` — zero mean, unit variance |
| Train-Test Split         | Held-out test set for unbiased evaluation   |

---

## 🧠 Model Architecture

| Layer          | Neurons | Activation |
| ---------------- | -------- | ------------ |
| Input Layer   | 11       | —            |
| Dense Layer   | 16       | ReLU         |
| Dense Layer   | 8        | ReLU         |
| Output Layer | 1        | Sigmoid      |

```
Input Layer (11 Features)
        ↓
Dense Layer (16 Neurons, ReLU)
        ↓
Dense Layer (8 Neurons, ReLU)
        ↓
Output Layer (1 Neuron, Sigmoid)
```

---

## ⚙️ Workflow

- Import Dataset
- Exploratory Data Analysis
- Data Cleaning
- Label Encoding
- One-Hot Encoding
- Train-Test Split
- Feature Scaling
- Build ANN using TensorFlow
- Compile Model
- Train Model
- Evaluate Performance
- Generate Predictions
- Save Trained Model

---

## 📈 Evaluation Metrics

| Metric                        | Interpretation                                          |
| -------------------------------- | ---------------------------------------------------------- |
| **Accuracy**                 | Proportion of correctly classified customers            |
| **Binary Cross Entropy** | Loss function for binary classification                 |
| **Confusion Matrix**       | Breakdown of true/false positives and negatives          |
| **Classification Report** | Precision, Recall, and F1-Score per class                |

---

## 🛠️ Tech Stack

| Category                | Libraries                     |
| -------------------------- | ------------------------------ |
| **Language**             | Python                         |
| **Deep Learning**    | TensorFlow, Keras              |
| **Data Manipulation** | Pandas, NumPy                  |
| **Visualization**      | Matplotlib, Seaborn            |
| **Machine Learning**  | Scikit-learn                   |
| **Environment**         | Jupyter Notebook               |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

```bash
# Clone the repository
git clone https://github.com/ChainForgeX/Customer_Churn_Prediction.git
cd Customer_Churn_Prediction

# Install dependencies
pip install -r requirement.txt
```

### Run the Project

```bash
jupyter notebook
```

Open `notebooks/Customer_Churn_Prediction.ipynb` and run all cells sequentially.

---

## 📸 Screenshots

### Churn Distribution (Exited)

[![Exited Distribution](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/exited.png)](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/exited.png)

### Epoch vs Accuracy

[![Epoch vs Accuracy](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/epoch_vs_accuracy.png)](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/epoch_vs_accuracy.png)

### Epoch vs Loss

[![Epoch vs Loss](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/epoch_vs_loss.png)](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/epoch_vs_loss.png)

### Confusion Matrix

[![Confusion Matrix](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/confusion_matrix.png)](https://github.com/ChainForgeX/Customer_Churn_Prediction/raw/main/images/confusion_matrix.png)

---

## 🎓 Skills Demonstrated

- Exploratory Data Analysis & Statistical Profiling
- Data Cleaning & Preprocessing
- Label Encoding & One-Hot Encoding
- Feature Scaling
- Artificial Neural Network Design
- Binary Classification with Sigmoid Activation
- Model Training & Hyperparameter Selection
- Model Evaluation (Accuracy, Confusion Matrix, Classification Report)
- Model Persistence with Keras
- Professional End-to-End Deep Learning Workflow

---

## 🔮 Future Improvements

- [ ] Hyperparameter Tuning
- [ ] Early Stopping
- [ ] Dropout Regularization
- [ ] Model Checkpointing
- [ ] TensorBoard Integration
- [ ] Deploy using FastAPI
- [ ] Docker Containerization

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Jeevan Yadav**
Computer Science Engineer | Blockchain Developer | AI & Machine Learning Enthusiast

[![Portfolio](https://img.shields.io/badge/Portfolio-000?style=flat&logo=vercel&logoColor=white)](https://jeevan-yadav.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-Jeevan9898-181717?style=flat&logo=github)](https://github.com/Jeevan9898)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jeevan_Yadav-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jeevan-yadav-b664952b5)

---

**⭐ If this project helped you understand the Deep Learning workflow for churn prediction, consider giving it a star.**
