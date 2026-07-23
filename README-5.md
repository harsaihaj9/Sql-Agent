# 📜 TaskBot - AI-Powered SQL Task Manager

An **Agentic AI** task management assistant that allows users to manage
tasks using **natural language** instead of writing SQL queries. Built
using **LangChain**, **LangGraph**, **Groq LLM**, **SQLite**, and
**Streamlit**.

------------------------------------------------------------------------

## 🚀 Features

-   Create, view, update, and delete tasks using natural language
-   Automatic SQL query generation and execution
-   Conversational interface with memory
-   Context-aware responses
-   Interactive Streamlit UI
-   SQLite-backed persistent storage

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   Python
-   Streamlit
-   LangChain
-   LangGraph
-   Groq LLM (GPT-OSS-20B)
-   SQLite
-   SQLDatabaseToolkit
-   python-dotenv

------------------------------------------------------------------------

## 🏗️ Architecture

``` text
User
  │
  ▼
Streamlit UI
  │
  ▼
LangChain Agent
  │
  ├── System Prompt
  ├── LangGraph Memory
  └── SQLDatabaseToolkit
          │
          ▼
      SQLite Database
          │
          ▼
      Generated Response
```

------------------------------------------------------------------------

## 📂 Project Structure

``` text
TaskBot/
├── app.py
├── my_tasks.db
├── .env
├── requirements.txt
└── README.md
```

------------------------------------------------------------------------

## ⚙️ Installation

``` bash
git clone https://github.com/your-username/taskbot.git
cd taskbot
pip install -r requirements.txt
streamlit run app.py
```

------------------------------------------------------------------------

## 🔑 Environment Variables

``` env
GROQ_API_KEY=your_groq_api_key
```

------------------------------------------------------------------------

## 💬 Example Prompts

-   Create a task to complete my assignment.
-   Show all pending tasks.
-   Mark task 3 as completed.
-   Delete task 5.

------------------------------------------------------------------------

## ✨ Highlights

-   Agentic AI Workflow
-   Natural Language to SQL (NL2SQL)
-   Automatic CRUD Operations
-   Prompt Engineering
-   Tool Calling
-   Conversation Memory
