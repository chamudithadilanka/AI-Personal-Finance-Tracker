💰 AI Personal Finance Tracker (CAIEP L1)

A chat-based personal finance assistant powered by an AI agent that understands natural language, manages your income & expenses, and gives smart financial insights.

<img width="1895" height="1018" alt="Screenshot 2026-04-29 185827" src="https://github.com/user-attachments/assets/d0ad1ff7-c793-4292-8517-92415e4f99b5" />
<img width="1886" height="986" alt="Screenshot 2026-04-29 185912" src="https://github.com/user-attachments/assets/591582c8-c93b-46e0-8f34-4d53ba71bd49" />
<img width="1888" height="912" alt="Screenshot 2026-04-29 190258" src="https://github.com/user-attachments/assets/a529ea96-c772-45d5-a9c4-69fe9b645fda" />
<img width="1867" height="888" alt="Screenshot 2026-04-29 190539" src="https://github.com/user-attachments/assets/c84b4d2f-54f8-4c20-8e4e-25186fae7acf" />
<img width="1806" height="956" alt="Screenshot 2026-04-29 190604" src="https://github.com/user-attachments/assets/bc995b64-cf1a-447a-8588-276c75c0b1b2" />
<img width="1896" height="936" alt="Screenshot 2026-04-29 191000" src="https://github.com/user-attachments/assets/edfdd226-b101-4b96-a5a0-f1421eaf6f3d" />
<img width="1852" height="927" alt="Screenshot 2026-04-29 191246" src="https://github.com/user-attachments/assets/01029089-b62f-4ab8-9d95-45f2d9071cc8" />
<img width="1825" height="872" alt="Screenshot 2026-04-29 191904" src="https://github.com/user-attachments/assets/c36c8b2f-a06a-48ac-990a-da65b5ca0933" />


Built as part of CAIEP L1 — Noob Dev Certified AI Engineer Program.

🚀 Features
💬 Chat-first interface (no forms, just conversation)
🧠 AI agent with tool calling
💵 Track monthly salary
📉 Track expenses
📊 Get balance & summaries
🗄️ Persistent SQLite database
🖥️ Simple Gradio UI
🧠 How It Works

The AI agent follows a loop:

User sends a message
AI understands intent
AI decides which tool to use
Tool executes (database read/write)
AI responds with a helpful message
🛠️ Tech Stack
Component	Tool
AI Model	Groq / OpenRouter / Ollama
UI	Gradio
Database	SQLite3
Backend	Python
Tool Calling	OpenAI-compatible API
📦 Project Structure
├── app.py                # Main application
├── database.db          # SQLite database
├── tools.py             # Tool functions
├── agent.py             # AI logic + tool loop
├── ui.py                # Gradio interface
└── README.md
⚙️ Setup Instructions
1. Clone the repository
git clone https://github.com/your-username/finance-tracker.git
cd finance-tracker
2. Install dependencies
pip install openai gradio sqlite3
3. Set API Key

For Groq:

export GROQ_API_KEY="your_api_key"

(Windows)

set GROQ_API_KEY=your_api_key
4. Run the app
python app.py
🗄️ Database Schema
Salary Table
Column	Type
id	INTEGER
amount	REAL
month	TEXT
year	INTEGER
created_at	TEXT
Expenses Table
Column	Type
id	INTEGER
amount	REAL
category	TEXT
description	TEXT
date	TEXT
🔧 Available Tools

The AI agent can call these functions:

set_salary(amount, month, year)
add_expense(amount, category, description, date)
get_expenses(month, year)
get_balance(month, year)
💬 Example Usage
User: My salary is 100000 for April 2026
AI: ✅ Salary recorded successfully!

User: I spent 2500 on food today
AI: 🍔 Expense added!

User: What's my balance this month?
AI: 💰 Your remaining balance is 75,000
🎯 Learning Objectives
Build a real AI agent
Implement tool calling
Work with SQLite databases
Create chat-based applications
Deploy AI-powered systems
⚠️ Disclaimer

This project is created for educational purposes as part of the Noob Dev CAIEP L1 program.

👨‍💻 Author

Chamuditha Dilanka
CAIEP L1 Student — Noob Dev

⭐ Support

If you like this project:

⭐ Star the repo
🍴 Fork it
🚀 Build your own version

screen shots

