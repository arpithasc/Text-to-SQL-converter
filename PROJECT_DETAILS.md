## 🏗️ System Architecture

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
