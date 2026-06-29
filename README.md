# Influencer_Fraud_Detection
🕵️ Influencer Fraud Detection EngineThis project is an AI-powered authenticity analysis system designed to identify fraudulent influencer activities, including fake followers, bot-driven engagement, and engagement manipulation. It helps brands ensure their marketing budgets are allocated to genuine partnerships by quantifying influencer authenticity. 
🛠️ Core Engineering & Methodology
Authenticity Metrics: The engine evaluates critical indicators such as follower-to-following ratios, engagement rates (comparing against industry standards of 1–5%), and follower growth velocity to detect anomalies. 
Behavioral Analysis: Using machine learning models, the system identifies bot-like patterns, such as coordinated engagement pods or unnatural audience demographics. 
Risk Scoring: The pipeline calculates an Authenticity Score (0–100) for each profile, classifying them into risk levels (e.g., Low, Medium, High, Critical) to streamline partnership decision-making.  
Red Flag Detection: Automatically flags suspicious account activity, such as recently created profiles with sudden high monetization, inconsistent posting frequency, or geographic mismatches between claimed and actual audience bases.
Interactive Demo: The project includes a Streamlit dashboard, enabling users to input influencer profiles and generate an immediate fraud assessment report.  
📁 Project Architecture
Plaintext
influencer-fraud-detection/
├── data/                    # (Ignored by .gitignore)
├── reports/                 # Logic for generating fraud assessments
├── src/                     # Source code (API connectors, analysis models)
├── app.py                   # Streamlit interactive dashboard
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
🚀 Setup and Execution Instructions
1. Environment SetupIt is recommended to use a virtual environment to manage dependencies for this project:
2. Bash# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # (On Windows use: venv\Scripts\activate)

# Install requirements
pip install -r requirements.txt
2. Launching the Analysis DashboardTo launch the dashboard to input an influencer’s handle and view their generated authenticity report:
Bashstreamlit run app.py
