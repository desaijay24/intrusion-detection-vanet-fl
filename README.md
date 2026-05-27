# Federated Learning Based Intrusion Detection and Prevention System for VANETs

A privacy-preserving Intrusion Detection and Prevention System (IDPS) for Vehicular Ad Hoc Networks (VANETs) using Federated Learning. This project demonstrates how distributed vehicular nodes can collaboratively train intrusion detection models without sharing raw network traffic data.

## Overview

Vehicular Ad Hoc Networks (VANETs) are a critical component of Intelligent Transportation Systems (ITS), enabling:

- Vehicle-to-Vehicle (V2V) communication
- Vehicle-to-Infrastructure (V2I) communication
- Real-time traffic coordination
- Enhanced road safety

However, VANETs are vulnerable to cyber threats such as:

- Denial of Service (DoS)
- Spoofing Attacks
- False Message Injection
- Routing Manipulation
- Probe Attacks

Traditional centralized IDS architectures require all vehicular data to be sent to a central server, causing:

- Privacy risks
- Scalability limitations
- Communication overhead
- Single point of failure

This project solves these challenges using Federated Learning (FL), where local vehicular nodes train models independently and only share model updates.

## Features

- Federated Learning–based IDS architecture
- Privacy-preserving distributed training
- Support for IID and Non-IID data distributions
- FedAvg aggregation algorithm
- FedProx aggregation algorithm
- Intrusion Prevention System (IPS)
- Mutual Information feature selection
- Scalable distributed training
- Reduced communication overhead
- High detection accuracy

## Technologies Used

### Machine Learning
- TensorFlow
- Keras
- Scikit-learn

### Federated Learning
- Flower (FLWR)

### Data Processing
- Pandas
- NumPy

### Visualization
- Matplotlib

### Development Environment
- Google Colab
- Python

## Dataset

Dataset Used:
- UNSW-NB15

The dataset contains:
- Normal network traffic
- Malicious traffic
- Flow-based network features
- Multi-class attack labels
  
## Project Workflow

### 1. Data Preprocessing
- Missing value handling
- Label encoding
- Feature normalization
- Standard scaling

### 2. Feature Selection
- Mutual Information–based feature selection
- Dimensionality reduction
- Communication cost reduction

### 3. Federated Learning Setup
- IID client distribution
- Non-IID client distribution
- Local client-side model training

### 4. Aggregation
- FedAvg for IID environments
- FedProx for Non-IID environments

### 5. Intrusion Prevention
- Normal traffic → ALLOW
- Malicious traffic → BLOCK

## Repository Structure

```text
intrusion-detection-vanet-fl/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   ├── preprocessing_feature_selection.ipynb
│   ├── iid_federated_learning.ipynb
│   └── non_iid_federated_learning.ipynb
│
├── dataset/
│   └── UNSW-NB15 Training and Testing Set.zip
│
├── images/
│   ├── architecture.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── results.png
