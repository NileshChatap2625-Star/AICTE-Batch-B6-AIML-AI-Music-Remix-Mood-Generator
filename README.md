📧 Email Assistant (AI-Based)

🚀 Automating email classification and actions using AI & Python

🧠 Overview

The Email Assistant is an AI-powered system that analyzes emails and automatically assigns actions such as:

📅 Schedule tasks
📤 Forward emails
🗂️ Organize inbox
📌 Mark personal emails

Built using the Enron Email Dataset, this project shows how automation improves productivity.

✨ Features
✅ Email dataset processing
✅ Automated action classification
✅ Gmail API integration
✅ Google Drive storage
✅ Data visualization (charts)
✅ Scalable AI logic
🏗️ Project Structure
email-assistant/
│── data/
│   └── emails.csv.zip
│
│── notebooks/
│   └── email_assistant.ipynb
│
│── output/
│   └── final_email_assistant.csv
│
│── src/
│   └── agent_logic.py
│
│── README.md
│── requirements.txt
⚙️ Installation
1️⃣ Clone Repository
git clone https://github.com/your-username/email-assistant.git
cd email-assistant
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Run Project
python main.py
🔑 Google Colab Setup
Authenticate Google Account
from google.colab import auth
auth.authenticate_user()
Mount Google Drive
from google.colab import drive
drive.mount('/content/drive')
📂 Dataset
Name: Enron Email Dataset
Format: CSV (zipped)
Contains:
Sender & Receiver
Subject & Date
Email content
Labels
⚡ Core Logic
def agent_action(row):
    if row['Cat_1_level_1'] == 1.0:
        return "Add to calendar / notify team"
    elif row['Cat_2_level_1'] == 1.0:
        return "Forward to accounts department"
    elif row['labeled'] == False:
        return "Mark as personal / no action"
    else:
        return "Archive"
📊 Output

📁 Final dataset stored at:

/content/drive/MyDrive/email dataset/final email assistant.csv

Includes:

Original email data
✅ New column: Agent_Action
📈 Visualization
📊 Pie chart showing distribution of email actions
