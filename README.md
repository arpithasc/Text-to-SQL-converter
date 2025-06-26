# 🧠 Text-to-SQL Query Converter 💬🗃️

A Natural Language Processing (NLP) based tool that translates **English text questions into SQL queries**. Designed to make database access easier for non-technical users by eliminating the need to write SQL manually.

## 🔍 Project Overview

This project allows users to:
- Enter a natural language question
- Automatically convert it to a valid SQL query
- Execute it on a predefined database schema (optional)
- Display the resulting table or output

## 💡 Features

- 🗣️ Natural language to SQL conversion
- 📄 Predefined database schema
- 🧠 Transformer or rule-based model
- 🖥️ User-friendly interface (Streamlit or Web GUI)
- ✅ SQL syntax validation

## 🛠️ Technologies Used

- **Python**
- **T5 / SQLNet / BERT (depending on implementation)**
- **SQLite / MySQL** (for testing query execution)
- **Streamlit / Flask** – Web interface
- **SQLAlchemy / sqlite3** – Database interaction

## 📁 Project Structure

```bash
Text-to-SQL/
│
├── models/                 # Trained NLP models (or checkpoints)
├── schema/                 # Sample database and schema definitions
├── queries/                # Input-output query logs
├── app.py                  # Main app interface
├── converter.py            # Text to SQL logic
├── executor.py             # Optional: Run generated SQL
├── requirements.txt        # Python dependencies
└── README.md               # You're here!


🏗️ System Architecture

The system is composed of the following key components:

1. **Input Module**  
   - Accepts natural language questions as input.
   - Optional: Accept voice input or load queries from a file.

2. **Preprocessing Engine**  
   - Tokenizes and normalizes the input sentence.
   - Identifies key entities and intent.

3. **Text-to-SQL Model**  
   - Trained transformer model (e.g., T5) that generates valid SQL queries based on input text and schema constraints.

4. **Database Schema Parser**  
   - Maps input queries to schema metadata to ensure syntactic and semantic validity.

5. **SQL Executor (Optional)**  
   - Executes the SQL query on a connected SQLite/MySQL database and returns results.

6. **Frontend Interface**  
   - Built using Streamlit or Flask for a clean, interactive experience.
   - Allows users to input queries, view generated SQL, and see query results.

