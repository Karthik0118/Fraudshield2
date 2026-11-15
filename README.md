# 🛡️ FraudShield
### Intelligent Financial Fraud Detection Support System

**An AI-powered cybersecurity application designed to detect fraudulent messages, analyze suspicious URLs, identify transaction network anomalies, and provide intelligent fraud assistance.**

---

## 📌 Overview

FraudShield is an intelligent financial fraud detection support system that leverages Machine Learning, Natural Language Processing (NLP), and Graph Convolutional Networks (GCN) to help users identify and understand potential financial fraud.

The system analyzes suspicious SMS messages, evaluates URL risk indicators, examines transaction networks, and provides AI-powered explanations to help users make safer digital financial decisions.

## ✨ Key Features

### 1. 📩 AI-Powered SMS Fraud Detection
- Detects fraudulent and suspicious SMS messages.
- Uses a fine-tuned DistilBERT transformer model.
- Classifies messages and provides fraud confidence scores.
- Helps users understand potential scam indicators.

### 2. 🔗 Intelligent URL Risk Analyzer
- Analyzes suspicious URLs.
- Evaluates multiple URL security indicators.
- Identifies potentially malicious links.
- Provides risk-based analysis.

### 3. 🧠 AI Fraud Assistant
- Interactive AI-powered chat interface.
- Explains why a message or activity may be suspicious.
- Provides fraud-related guidance and recommendations.
- Supports contextual fraud explanations.

### 4. 🌐 Transaction Network Analysis
- Uses Graph Convolutional Networks (GCN).
- Analyzes financial transaction relationships.
- Helps identify suspicious transaction patterns.
- Supports CSV, JSON, and PDF-based analysis workflows.

### 5. 📊 Detection History
- Maintains a history of fraud detection activities.
- Allows users to review previous detection results.

### 6. 🔐 User Profile & Security
- User profile management.
- Settings and preferences.
- Password management.
- Permission and security controls.

---

## 🛠️ Technology Stack

| Component | Technologies |
|---|---|
| Mobile Application | React Native, TypeScript |
| Backend | Node.js, Express.js |
| Machine Learning API | Python, FastAPI |
| NLP Model | DistilBERT |
| Deep Learning | PyTorch |
| Network Analysis | Graph Convolutional Networks (GCN) |
| Database | MongoDB |
| Development Tools | Android Studio, VS Code, Git |

---

## 🏗️ System Architecture

```text
              FRAUDSHIELD
                   |
          React Native Mobile App
                   |
             Node.js Backend
              (Port 5000)
                   |
        +----------+----------+
        |          |          |
     MongoDB    FastAPI    AI Assistant
                (8000)         |
                  |        Explanations
           +------+------+
           |             |
        DistilBERT      GCN
           |             |
        SMS Fraud    Transaction
        Detection     Analysis
           |
       Prediction
           |
      Mobile App
```

---

## 📂 Project Structure

```text
FraudShield/
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── services/
│   └── server.js
│
├── model/
│   ├── main.py
│   └── requirements.txt
│
├── MyApp/
│   ├── src/
│   │   ├── components/
│   │   ├── navigation/
│   │   ├── screens/
│   │   └── theme/
│   ├── android/
│   └── package.json
│
├── fraudshield-network-analysis/
│
├── start.bat
└── README.md
```

*Individual folder contents may vary depending on the latest development version.*

---

## ⚙️ Installation & Setup

### Prerequisites

Install the following:

- Node.js and npm
- Python 3.x
- MongoDB
- Android Studio
- Android SDK and ADB
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/Karthik0118/Fraudshield2.git
cd Fraudshield2
```

### 2. Start MongoDB

Make sure your local MongoDB service is running.

### 3. Start Backend Server

```powershell
cd backend
npm install
npm start
```

Backend runs on:

`http://localhost:5000`

### 4. Start Machine Learning API

Open another terminal:

```powershell
cd model
```

Activate your Python virtual environment:

```powershell
.\venv\Scripts\activate
```

Install dependencies if required:

```powershell
pip install -r requirements.txt
```

Start FastAPI:

```powershell
uvicorn main:app --host 0.0.0.0 --port 8000 --reload
```

API documentation:

`http://localhost:8000/docs`

### 5. Start React Native Application

Open another terminal:

```powershell
cd MyApp
npm install
```

Connect your Android device with USB debugging enabled.

```powershell
adb devices
```

Configure port forwarding:

```powershell
adb reverse tcp:5000 tcp:5000
adb reverse tcp:8000 tcp:8000
adb reverse tcp:8081 tcp:8081
```

Start Metro:

```powershell
npx react-native start
```

Open another terminal:

```powershell
cd MyApp
npx react-native run-android
```

---

## 📸 Application Screenshots

Add your actual application screenshots below.

| Application | Screenshot |
|---|---|
| Splash Screen | `report_screenshots/01_Splash_Screen.png` |
| Login Screen | `report_screenshots/02_Login_Screen.png` |
| Registration | `report_screenshots/03_Register_Screen.png` |
| Home Dashboard | `report_screenshots/04_Home_Dashboard.png` |
| SMS Scanner | `report_screenshots/05_SMS_Scanner_Screen.png` |
| Network Analysis | `report_screenshots/06_GCN_Network_Analysis_Screen.png` |
| AI Assistant | `report_screenshots/08_AI_Assistant_Chat_Screen.png` |
| User Profile | `report_screenshots/10_User_Profile_Screen.png` |

---

## 🔬 Machine Learning Approach

### SMS Fraud Detection

FraudShield uses a DistilBERT-based transformer model:

`mariagrandury/distilbert-base-uncased-finetuned-sms-spam-detection`

The model processes SMS text and generates classification predictions with confidence scores.

### Transaction Network Analysis

The network analysis component uses Graph Convolutional Networks to examine relationships between financial transactions and identify potentially suspicious patterns.

### URL Risk Analysis

The URL analyzer evaluates multiple security indicators to estimate the risk associated with suspicious links.

---

## 🎯 Project Objectives

1. Develop an intelligent system for detecting fraudulent SMS messages.
2. Identify potentially malicious URLs through automated risk analysis.
3. Apply graph-based learning to financial transaction analysis.
4. Provide understandable fraud explanations through an AI assistant.
5. Build an integrated mobile platform for fraud detection and awareness.

---

## 🔮 Future Enhancements

- Real-time fraud monitoring.
- Advanced financial transaction anomaly detection.
- Improved fraud classification accuracy.
- Enhanced explainable AI capabilities.
- Expanded integration with financial security systems.

---

## 👨‍💻 Developer

**Karthik**

GitHub: [@Karthik0118](https://github.com/Karthik0118)

Project Repository: [Fraudshield2](https://github.com/Karthik0118/Fraudshield2)

---

## 📄 License

This project is developed for academic and research purposes.

---

**FraudShield – Detect. Analyze. Protect.**

*Building a safer digital financial ecosystem through Artificial Intelligence.*
