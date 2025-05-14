# Fraud Detection System

A machine learning-based fraud detection system with a Streamlit web interface for real-time transaction analysis.

## Overview
This system uses a logistic regression model trained on transaction data to detect potentially fraudulent transactions. The web interface allows users to input transaction details and receive immediate fraud risk assessment.

## Features
- Interactive web interface using Streamlit
- Machine learning model for fraud detection
- Support for multiple transaction types
- Real-time prediction capabilities
- Balance tracking for both sender and receiver
- Visual feedback for prediction results

## Prerequisites
- Python 3.12 or higher
- pip package manager
- Required Python packages (listed in requirements.txt)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Fraud-Detection-System
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Running the Application

1. Start the Streamlit web interface:
```bash
streamlit run fraud_detection.py
```

2. Access the application in your web browser at:
```
http://localhost:8501
```

## Using the Application

1. Enter transaction details:
   - Select transaction type (PAYMENT, TRANSFER, CASH_OUT, DEPOSIT)
   - Enter transaction amount
   - Input sender's old and new balance
   - Input receiver's old and new balance

2. Click "Predict" to get fraud assessment

3. View results:
   - Green message for legitimate transactions
   - Red warning for potentially fraudulent transactions

## Project Structure
```
Fraud-Detection-System/
├── fraud_detection.py      # Main Streamlit application
├── analysis_model.ipynb    # Model training notebook
├── requirements.txt        # Project dependencies
├── fraud_detection_model.pkl   # Trained model file
├── LICENSE
└── README.md
```

## Model Details
- Algorithm: Logistic Regression
- Features used:
  - Transaction type
  - Transaction amount
  - Sender's balance (before and after)
  - Receiver's balance (before and after)
- Training data: Financial transaction dataset with labeled fraud cases

## Troubleshooting

If you encounter "command not found" errors:
```bash
# Install pipx
sudo apt install pipx
pipx ensurepath

# Install Streamlit globally
pipx install streamlit
```

## Contributing
Feel free to submit issues and enhancement requests.

## Contact
For any inquiries, please reach out to:
- Email: marcpon8@gmail.com
- GitHub: https://github.com/poncema4
