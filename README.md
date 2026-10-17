# VisionVault – AI-Powered Privacy-Aware Data Leakage Prevention Gateway

## About the Project

VaultVision is an AI-powered data security project designed to detect sensitive information in text and help prevent accidental data leakage. It identifies potentially confidential information such as email addresses, phone numbers, passwords, and API keys before the data is shared.

The project combines rule-based pattern detection and Machine Learning to classify text as **Safe** or **Sensitive** and assign a risk level to help determine whether the data should be allowed, reviewed, or blocked.

## Objectives

- Detect sensitive information in text.
- Identify potential data leakage risks.
- Classify text as Safe or Sensitive using Machine Learning.
- Calculate risk scores based on detected information.
- Provide gateway decisions to improve data protection.
- Visualize scan history and risk analysis through charts.

## Features

- **Sensitive Data Detection:** Detects emails, phone numbers, passwords, and API keys.
- **Machine Learning Classification:** Uses TF-IDF and Logistic Regression to classify text.
- **Risk Scoring:** Assigns risk scores based on detected sensitive information.
- **Security Decisions:** Generates ALLOWED, REVIEW REQUIRED, or BLOCKED decisions based on configured rules.
- **Interactive Scanner:** Allows users to scan text and review the results.
- **Dashboard & Analytics:** Displays scan summaries, detection charts, risk distributions, and scan history.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- ipywidgets
- Regular Expressions (Regex)

## How It Works

1. The user enters text into the scanner.
2. The system scans the text for sensitive information using predefined patterns.
3. The Machine Learning model classifies the text as Safe or Sensitive.
4. A risk score is calculated according to the detected information.
5. The system generates a security decision: ALLOWED, REVIEW REQUIRED, or BLOCKED.
6. The results are displayed for analysis and monitoring.

## Risk Scoring

The prototype uses configurable risk scores for selected data types:

| Sensitive Data Type | Risk Score |
|---|---:|
| Email Address | 20 |
| Phone Number | 30 |
| API Key | 50 |

Risk levels and gateway decisions depend on the rules configured in the project.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/VaultVision.git
```

### 2. Open the Project Folder

```bash
cd VaultVision
```

### 3. Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib ipywidgets jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells in order.

## Dashboard & Analytics

The project includes visualizations for:

- Total scans and summary metrics
- Sensitive data detection counts
- Low, Medium, and High risk distribution
- Risk scores across individual scans
- Scan history and analysis results

## Security Note

VaultVision is an educational prototype. It is not a production-ready data loss prevention system. Pattern-based detection and Machine Learning can produce false positives and false negatives. Do not use real passwords, API keys, or other confidential information while testing.

## Future Improvements

- Real-time monitoring of outgoing data
- Advanced sensitive data detection using NLP
- Web-based dashboard using Streamlit
- Secure logging and audit reports
- Customizable security policies and risk thresholds
- Integration with enterprise applications

## Acknowledgements

This project was developed as a learning initiative in Python, Machine Learning, data security, and data visualization.

If you find this project useful, consider giving the repository a star!
