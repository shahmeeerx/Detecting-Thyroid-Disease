# Thyroid Disease Prediction using Artificial Neural Networks (ANN)

> **A diagnostic machine learning model developed in MATLAB to automate the detection of thyroid disorders using clinical patient indicators.**

##  Project Overview
Thyroid disorders are prevalent endocrine conditions that often go undiagnosed due to overlapping symptoms. This project implements a **Feedforward Artificial Neural Network (ANN)** to classify patients as either "Normal" or "Positive for Thyroid Disease". 

By utilizing **MATLAB’s Neural Network Toolbox**, the model identifies complex, non-linear relationships between 11 medically significant attributes—such as age, gender, medication usage, and hormonal indicators—to provide an accurate binary diagnosis.


## 🛠️ Technical Specifications
* **Platform:** MATLAB R2019b.
* **Toolbox:** Neural Network Toolbox via the `nnstart` (Pattern Recognition) App.
* **Architecture:** Multilayer Perceptron (MLP).
  * **Input Layer:** 11 neurons representing individual clinical features.
  * **Hidden Layer:** 10 neurons with **logsig** activation functions.
  * **Output Layer:** 1 neuron with **sigmoid/logsig** activation for binary classification.
* **Training Algorithm:** Scaled Conjugate Gradient (`trainscg`).
* **Loss Function:** Cross-Entropy.

## Clinical Dataset & Preprocessing
The model was trained on a curated subset of the **UCI Thyroid Disease dataset**.
* **Features Used:** Gender, Age > 30, On Thyroxine, Anti-thyroid Medication, Goitre, Tumor, Pregnancy Status, Sick status, Thyroid Surgery history, Hypopituitary dysfunction, and Psychiatric history.
* **Encoding:** Categorical and demographic data were converted into **Binary Encoding** (0 or 1) to ensure computational efficiency and compatibility with the network.
* **Data Split:** 70% Training, 15% Validation, and 15% Testing.

## Performance & Results
The model demonstrated perfect classification within the scope of the training environment, achieving **100% accuracy** across all data subsets.

| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **Overall Accuracy** | **100%** | All samples correctly classified. |
| **Best Validation Perf.** | **0.008543** | Minimum cross-entropy loss at Epoch 25. |
| **Misclassifications** | **0** | No false positives or false negatives detected. |
| **Final Gradient** | **9.17 × 10⁻⁷** | Training halted upon meeting gradient threshold. |


## Development Team
* **Shahmeer Hussain** — [@shahmeeerx](https://github.com/shahmeeerx) (2022F-BBM-014)
* **Amna Yousuf Judge** — [@amna-014](https://github.com/amna-014) (2022F-BBM-012)
* **Sabeen Ansari** — (2022F-BBM-035)

---
_© 2026 Thyroid Disease Prediction Project. Developed for the Dept. of Biomedical Engineering, SSUET._
