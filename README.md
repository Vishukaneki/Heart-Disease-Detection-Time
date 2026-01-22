# Heart Disease Detection System (BTP 2025)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange)
![Status](https://img.shields.io/badge/Status-Active-success)

## 📌 Project Overview
This repository contains the source code and datasets for a **Heart Disease Detection System**, developed as a Bachelor of Technology Project (BTP 2025). 

The project goes beyond simple classification by implementing a **multi-stage data engineering pipeline**. It utilizes unsupervised learning (Clustering) to augment the dataset before feeding it into supervised learning models (XGBoost, Random Forest, and ANN) to predict Coronary Output (0: Healthy, 1: At Risk).

## 📂 Repository Structure

The project is organized into specific modules for data processing, training, and reporting:

| File / Directory | Description |
| :--- | :--- |
| **`coronaryHealth (1).ipynb`** | The main Jupyter Notebook containing the End-to-End pipeline (EDA, Preprocessing, Modeling). |
| **`Neural Network/`** | Contains the Deep Learning architecture definitions and saved model weights. |
| **`BtpReport2k25.docx`** | Official project report detailing the methodology, mathematical foundations, and final results. |
| **`Filtered_Cardiac_Data.csv`** | The initial cleaned and preprocessed dataset. |
| **`Clustered_Cardiac_Data.csv`** | Dataset augmented with cluster labels (unsupervised learning) to capture non-linear patient groupings. |
| **`Optimized_Cardiac_Data.csv`** | The final dataset post-feature selection/optimization, used for high-performance training. |
| **`heartInformation.txt`** | Metadata explaining the clinical features used in the analysis. |

## ⚙️ Methodology

### 1. Data Engineering Pipeline
* **Filtration:** Handling missing values and removing statistical outliers.
* **Clustering-Based Augmentation:** Applied **K-Means Clustering** to segment patients into distinct profiles. These cluster labels were added as new features to help the model learn complex decision boundaries.
* **Optimization:** Feature selection was performed to reduce dimensionality and noise, resulting in the `Optimized_Cardiac_Data` set.

### 2. Model Architectures
We benchmarked three distinct architectures to ensure reliability:
* **Artificial Neural Network (ANN):** A Deep Learning approach using Dense layers to capture high-dimensional patterns.
* **XGBoost:** Gradient boosting framework optimized for speed and performance on tabular data.
* **Random Forest:** Ensemble learning method used as a robust baseline to prevent overfitting.

## 🚀 How to Run

### Prerequisites
* Python 3.8+
* Jupyter Notebook or Google Colab

### Installation
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Vishukaneki/Heart-Disease-Detection-Time.git](https://github.com/Vishukaneki/Heart-Disease-Detection-Time.git)
    cd Heart-Disease-Detection-Time
    ```

2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn tensorflow xgboost
    ```

3.  **Execute the Pipeline:**
    Run the main notebook to reproduce the training and evaluation steps:
    ```bash
    jupyter notebook "coronaryHealth (1).ipynb"
    ```

## 📊 Results & Analysis
The models were evaluated based on **Accuracy**, **Precision**, **Recall**, and **F1-Score**. 
* *For a detailed breakdown of the confusion matrices and ROC curves, please refer to `BtpReport2k25.docx`.*

## 👤 Author
**Vishal (VishuKaneki)**
* SDE | Instrumentation & Control Engineering

---
