# Unsupervised Credit Card Fraud Detection

An unsupervised machine learning project that identifies potentially fraudulent credit card transactions using clustering and anomaly detection techniques. Since fraud labels are assumed to be unavailable during model training, the project focuses on detecting anomalies based on transaction patterns and evaluates the models using the true labels only after training.

---

## Project Overview

Financial fraud is a major challenge due to the rarity of fraudulent transactions and the lack of labeled data in many real-world scenarios. This project applies unsupervised learning algorithms to detect suspicious transactions without using fraud labels during model development.

The project compares two popular unsupervised approaches:

- **K-Means Clustering**
- **Isolation Forest**

The fraud labels are used only for evaluating model performance.

---

## Objectives

- Understand the structure of a real-world fraud detection dataset.
- Perform exploratory data analysis (EDA).
- Preprocess and scale transaction features.
- Detect anomalous transactions using unsupervised learning.
- Compare clustering and anomaly detection techniques.
- Evaluate results using Precision, Recall, and Confusion Matrix.

---

## Dataset

**Dataset:** Credit Card Fraud Detection Dataset

- Source: Kaggle
- Total Transactions: **284,807**
- Fraud Cases: **492**
- Features: **31**

Features include:

- Time
- V1 – V28 (PCA-transformed features)
- Amount
- Class (used only for evaluation)

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Machine Learning Techniques

### 1. Exploratory Data Analysis

- Dataset overview
- Missing value analysis
- Feature distributions
- Class imbalance visualization
- Correlation analysis

### 2. Data Preprocessing

- Feature scaling using StandardScaler
- Separation of features and labels
- Optional dimensionality reduction using PCA

### 3. K-Means Clustering

- Cluster transactions into two groups
- Interpret clusters
- Visualize clustering results

### 4. Isolation Forest

- Detect anomalous transactions
- Predict suspicious observations
- Compare anomaly distribution

---

## Evaluation Metrics

Although the project follows an unsupervised approach, the original fraud labels are used after training for evaluation.

Metrics include:

- Confusion Matrix
- Precision
- Recall

---

## Project Structure

```
Unsupervised-Fraud-Detection/
│
├── creditcard.csv
├── ML_Fraud_Project.ipynb
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Unsupervised-Fraud-Detection.git
```

Navigate to the project directory:

```bash
cd Unsupervised-Fraud-Detection
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
ML_Fraud_Project.ipynb
```

---

## Results

The project compares K-Means Clustering and Isolation Forest for identifying fraudulent transactions.

**Key observations:**

- K-Means groups transactions based on similarity but struggles with highly imbalanced datasets.
- Isolation Forest effectively isolates rare observations, making it more suitable for fraud detection.
- Isolation Forest demonstrates better anomaly detection performance in this dataset.

---

## Future Improvements

- Implement DBSCAN for density-based anomaly detection.
- Explore Autoencoders for deep anomaly detection.
- Tune Isolation Forest hyperparameters.
- Build an interactive fraud monitoring dashboard.
- Deploy the model using Flask or FastAPI.

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Unsupervised Machine Learning
- Fraud Detection
- Anomaly Detection
- Clustering Algorithms
- Data Preprocessing
- Exploratory Data Analysis
- Model Evaluation
- Financial Data Analytics

---

## Author

**Devisha Jain**

B.Tech Computer Science (Data Science)  
Manipal University Jaipur

---

## License

This project is developed for educational purposes.
