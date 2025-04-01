# 🤖 Federated Learning with UCI Adult Dataset

## 📌 Project Description
This project explores **federated learning** using the **UCI Adult dataset**, implementing **horizontal, vertical, and transversal federated learning**. Additionally, it features a specialized **horizontal federated learning approach with smart contracts**, leveraging **Web3, Ngrok, Remix IDE, and Ganache** to integrate blockchain-based security.

## 🚀 Features
- 🔄 **Horizontal, Vertical, and Transversal Federated Learning**
- 🔗 **Smart Contract Implementation for Secure Federated Learning**
- 🏛 **Uses Web3, Ngrok, Remix IDE, and Ganache for Decentralization**
- 🔬 **Privacy-Preserving Machine Learning Techniques**
- 📊 **Evaluates Model Performance Across Federated Scenarios**

## 🛠 Installation
Install the required dependencies:

```bash
pip install tensorflow torch numpy pandas scikit-learn flwr web3
```

For the blockchain-based implementation, install Ganache and set up Web3:

```bash
npm install -g ganache-cli
pip install web3
```

## 📂 Dataset
The project uses the **UCI Adult dataset**, which can be downloaded from:

[UCI Machine Learning Repository - Adult Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data)

To load and preprocess the dataset:

```python
from data_preprocessing import load_adult_data
df = load_adult_data("adult.data")
print(df.head())
```

## 🎯 Model Training
### Federated Learning Training
Run the federated learning model with:

```bash
python federated_train.py --mode horizontal
python federated_train.py --mode vertical
python federated_train.py --mode transversal
```

### Blockchain-Based Horizontal FL Training
To execute the **smart contract-based** training:

```bash
python smart_contract_fl.py --ganache --ngrok
```

## 🔍 Usage
To predict an individual's income category using the federated learning model:

```python
from predictor import predict_income
sample_data = {"age": 35, "education": "Bachelors", "hours_per_week": 40}
result = predict_income(sample_data)
print("Prediction:", result)
```

## 📈 Evaluation
The model's performance is evaluated using:
- ✅ **Accuracy**
- 📉 **Precision, Recall, and F1-score**
- 🔗 **Smart Contract Audit for Security Analysis**

## 🙌 Acknowledgments
- 🏛 **Flower (FLWR)** for federated learning framework
- 🔗 **Ethereum & Web3** for smart contract integration
- 📊 **UCI Machine Learning Repository** for dataset
