# Chat with SQL Database
This application allows you to chat with an SQL database (either SQLite or MySQL) using a LangChain-based agent with a Groq-powered LLM (Llama3-8b-8192). The app is built using Streamlit, which provides a simple and interactive interface.

## Features
- `Database Connectivity`: Supports both SQLite and MySQL databases.
- `SQL Querying`: You can interact with your database using natural language queries.
- `Groq LLM Integration`: The app uses the Groq API to run an LLM model (Llama3-8b-8192) to interpret and generate responses.
- `Streamlit UI`: A web-based interface that facilitates seamless communication with the database.
## Setup Instructions

### 1. Install dependencies
Make sure you have `streamlit, langchain`, and other required Python packages installed. You can install them using the following command:
```bash
pip install -r requirements.txt
```
### 2. Configuration
- **SQLite**: The app uses a local SQLite database (student.db). Ensure that the database file is located in the root directory of the project.
- **MySQL**: If you choose MySQL, you need to provide the following details:
- MySQL Host
- MySQL User
- MySQL Password
- MySQL Database Name

### 3. Groq API
You will need a `Groq API key` to use the LLM. This can be entered in the sidebar once the app is running. Visit the [Groq](https://groq.com/) Website.

### 4. Running the App
Once you've set up your environment and configured the database, run the Streamlit app with the following command:
```bash
streamlit run app.py
```
Or you can check the app here: [Chat with SQL](https://langchain-with-sql-32uzvwjd79zyhukrar8z6x.streamlit.app/)

### 5. Interacting with the App
- Choose the database (SQLite or MySQL) from the sidebar.
- Provide your Groq API key to enable the language model functionality.
- Ask questions directly in the chatbox, and the LLM will query the database to provide the response.

### Requirements
- Python 3.x
- Streamlit
- LangChain
- SQLAlchemy
- sqlite3 (for local SQLite)
- MySQL (optional for MySQL use)
- Groq API Key

### Files
You can use `sqlite.py` to create a local sqlite file so that can you use it in the app.
