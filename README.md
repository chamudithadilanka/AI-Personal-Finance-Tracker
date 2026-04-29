💰 AI Personal Finance Tracker (CAIEP L1)

A chat-based personal finance assistant powered by an AI agent that understands natural language, manages your income & expenses, and gives smart financial insights.

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

