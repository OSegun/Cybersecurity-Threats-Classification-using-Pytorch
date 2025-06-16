# Cybersecurity-Threats-Classification-using-Pytorch

This project is a proof-of-concept (POC) deep learning system for detecting and classifying cyber threats. With the rise in frequency and sophistication of cyber-attacks such as malware, phishing, and denial-of-service (DoS), traditional detection methods often fall short. This model development with pytorch is designed to enhance an organization’s cybersecurity readiness by proactively identifying these threats using data-driven approaches.

The system leverages deep learning techniques with pytorch framework to analyze structured security event data and classify whether an activity poses a cyber threat or not.

## 📂 Project Structure

- `notebook.ipynb`: Main notebook containing the entire workflow—data loading, preprocessing, model development, and evaluation.
- `labelled_train.csv`, `labelled_test.csv`, `labelled_validation.csv`: Datasets containing labeled network or system event logs.


## 📊 Problem Description

The task is to classify cybersecurity incidents into categories such as malicious or benign, based on network activity, user behavior, or system metrics.

Each sample includes:
- Structured data features representing the security context.
- A target label indicating whether the event is a threat.

The project uses PyTorch to build, train, and evaluate the neural network classifier.

## 🧱 Dataset

The dataset is structured in CSV format:
- `labelled_train.csv`: Used for training the model.
- `labelled_test.csv`: Used for evaluating generalization.
- `labelled_validation.csv`: Used for tuning and early stopping.

Preprocessing steps include:
- Feature standardization with `StandardScaler`.
- Conversion to PyTorch tensors for model training.

## ⚙️ Dependencies

Ensure the following packages are installed:

```bash
torch
torchmetrics
pandas
scikit-learn