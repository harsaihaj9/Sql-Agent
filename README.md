# TaskBot - AI-Powered SQL Task Manager

An intelligent **Agentic AI** task management assistant that enables users to manage tasks using **natural language** instead of writing SQL queries. Built using **LangChain**, **LangGraph**, **Groq LLM**, **SQLite**, and **Streamlit**.

---

##  Features

-  Create tasks using natural language
-  View existing tasks
-  Update task status
-  Delete tasks
-  Conversational chat interface
-  Context-aware conversations using memory
-  Automatic SQL generation and execution
-  Tasks displayed in a structured format

---

##  Tech Stack

- **Python**
- **LangChain**
- **LangGraph**
- **Groq LLM (GPT-OSS-20B)**
- **SQLite**
- **SQLDatabaseToolkit**
- **Streamlit**
- **python-dotenv**

---

##  Architecture

```
          User
            │
            ▼
     Streamlit Chat UI
            │
            ▼
      LangChain Agent
            │
    ┌───────┴────────┐
    │                │
System Prompt     Conversation Memory
                    (LangGraph)
    │                │
    └───────┬────────┘
            │
            ▼
   SQLDatabaseToolkit
            │
            ▼
        SQLite Database
            │
            ▼
       Generated Response
```

---

##  Project Structure

```
TaskBot/
│── app.py
│── .env
│── my_tasks.db
│── requirements.txt
└── README.md
```

---

##  Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/taskbot.git

cd taskbot
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Windows

```bash
venv\Scripts\activate
```

Mac/Linux

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

##  Environment Variables

Create a `.env` file in the project root.

```env
GROQ_API_KEY=your_groq_api_key
```

---

##  Run the Application

```bash
streamlit run app.py
```

---

## Example Prompts

```
Create a task to complete my DBMS assignment.

Show all pending tasks.

Mark task 3 as completed.

Update "Buy Groceries" to in_progress.

Delete task 5.

Show my latest tasks.
```

---

##  How It Works

1. User enters a request in natural language.
2. LangChain Agent interprets the request.
3. SQLDatabaseToolkit converts it into SQL operations.
4. SQLite executes the query.
5. LangGraph maintains conversation memory.
6. Results are returned through the Streamlit interface.

---

##  Key Highlights

- Agentic AI workflow
- Natural Language to SQL (NL2SQL)
- Automatic CRUD operations
- Conversation memory
- Prompt engineering
- SQL tool calling
- Interactive Streamlit UI

---

##  Demo

_Add screenshots or a GIF here._

---

##  Future Enhancements

- User authentication
- Multi-user task management
- Task priorities
- Due dates & reminders
- Calendar integration
- Email notifications
- PostgreSQL/MySQL support
- Docker deployment

---

