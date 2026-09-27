# Influence Guard AI

## AI-Powered Influencer Fraud Detection & Creator Authenticity Analysis Platform

Influence Guard AI is a Streamlit-based platform designed to analyze
YouTube creator data, identify suspicious engagement patterns, and
assess creator authenticity using data analysis and machine-learning
techniques.

## 🚀 Features

-   🔍 YouTube channel analysis
-   🤖 AI-based fraud and anomaly detection
-   📊 Creator engagement and performance metrics
-   🛡️ Suspicious creator identification
-   📈 Fraud score and influence score calculation
-   👤 User authentication
-   🗄️ MySQL database integration
-   📋 Analysis history and reports
-   🎨 Interactive Streamlit dashboard

## 🧠 Project Workflow

1.  User logs into the application.
2.  User enters a YouTube Channel URL or Channel ID.
3.  The application retrieves publicly available channel information
    using YouTube Data API v3.
4.  Creator metrics are processed using Python and Pandas.
5.  Engagement and growth-related indicators are calculated.
6.  The system generates fraud and influence scores.
7.  Creator authenticity is classified based on the analyzed indicators.
8.  Analysis results can be stored in MySQL for history and reporting.

## 🛠️ Tech Stack

  Technology            Purpose
  --------------------- ----------------------------------------
  Python                Core programming and data processing
  Streamlit             Web application and interactive UI
  Pandas                Data processing and analysis
  NumPy                 Numerical operations
  Scikit-learn          Machine learning and anomaly detection
  MySQL                 Database management
  MySQL Connector       Python-MySQL connectivity
  YouTube Data API v3   YouTube creator data retrieval
  Joblib                ML model persistence
  HTML/CSS              UI styling

## 📊 Analysis Metrics

The platform works with creator-level indicators such as:

-   Subscriber/follower count
-   Likes
-   Comments
-   Shares
-   Saves
-   Followers gained
-   Engagement ratio
-   Growth rate
-   Fraud score
-   Influence score
-   Fake/suspicious follower estimation
-   Creator/account status

## 🤖 Fraud & Anomaly Detection

The project combines rule-based indicators with machine-learning-based
anomaly detection.

Indicators include:

-   Very low engagement compared with audience size
-   Low engagement patterns
-   Unusually high growth
-   Unusual like-to-audience ratios
-   Very low overall interaction

For datasets containing multiple records, the project can use
Scikit-learn's Isolation Forest for anomaly detection. For single-record
creator analysis, rule-based scoring is used.

> Note: Fraud scores and authenticity indicators are analytical
> estimates based on the implemented project logic. They should not be
> treated as definitive proof that an individual creator has fake
> followers or fraudulent activity.

## 🗂️ Project Structure

``` text
Influence-Guard-AI/
├── .streamlit/
│   └── config.toml
├── assets/
├── components/
│   └── ui.py
├── database/
├── pages/
├── styles/
├── utils/
├── app.py
├── auth.py
├── database.py
├── insights.py
├── model.py
├── model.pkl
├── youtube_api.py
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Local Setup

### 1. Clone the repository

``` bash
git clone https://github.com/Shivanii909/Influence-Guard-AI.git
cd Influence-Guard-AI
```

### 2. Create a virtual environment

Windows:

``` powershell
python -m venv venv
venv\Scriptsctivate
```

### 3. Install dependencies

``` powershell
pip install -r requirements.txt
```

### 4. Configure secrets

Create:

``` text
.streamlit/secrets.toml
```

Add your YouTube API key:

``` toml
YOUTUBE_API_KEY = "YOUR_API_KEY_HERE"
```

Do not upload `secrets.toml` to GitHub.

### 5. Run the application

``` powershell
python -m streamlit run app.py
```

## 🔐 Security

API keys and database credentials should be stored in Streamlit secrets
or environment variables.

Never commit API keys, database passwords, or other credentials to
GitHub.

## 📌 Project Purpose

This project demonstrates practical skills in:

-   Python programming
-   Data analysis
-   Machine learning
-   Anomaly detection
-   API integration
-   SQL/MySQL database management
-   Streamlit application development
-   Data-driven decision support

## 👩‍💻 Author

**SHIVANI**

Aspiring Data Analyst & Business Intelligence Analyst

### Skills

Python • SQL • Pandas • NumPy • Power BI • Tableau • Streamlit •
Scikit-learn • MySQL • Data Analysis • Machine Learning • Data
Visualization

## 🔗 Repository

GitHub: https://github.com/Shivanii909/Influence-Guard-AI
Linkedln: https://www.linkedin.com/in/shivani-a07857423
