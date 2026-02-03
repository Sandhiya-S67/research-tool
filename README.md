# AtliQ Tees: Talk to a Database

This project is an end-to-end **LLM-powered application** that allows users to interact with a **MySQL database using natural language**.
Instead of writing SQL queries manually, users can ask questions in plain English, and the system automatically generates and executes the required SQL queries to produce accurate answers.

AtliQ Tees is a T-shirt retail store where inventory, sales, and discount information are stored in a MySQL database.
The system is designed to help store managers quickly retrieve business insights without technical effort.

A store manager can ask questions like:

* How many Adidas white T-shirts are currently in stock?
* What will be the total sales if all extra-small T-shirts are sold after discounts?

The system understands the question, generates the correct SQL query, executes it, and displays the result.

---

## Project Highlights

* AtliQ Tees is a retail store selling:

  * Adidas
  * Nike
  * Van Heusen
  * Levi’s

* All inventory, sales, and discount data are maintained in a **MySQL database**

* An LLM-based Question Answering system is built using:

  * Google PaLM language model
  * Hugging Face embeddings
  * LangChain framework
  * ChromaDB vector store
  * Streamlit for the user interface
  * Few-shot learning for better accuracy

* Users can ask questions in **natural language**

* The system responds with database-driven answers

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Sandhiya-S67/research-tool.git
```

2. Navigate to the project directory:

```bash
cd research-tool
```

3. Install required dependencies:

```bash
pip install -r requirements.txt
```

4. Generate a Google API key from:

```
https://makersuite.google.com
```

5. Create a `.env` file and add the API key:

```env
api_key="your_api_key_here"
```

6. Set up the database by executing:

```
database/db_creation_atliq_t_shirts.sql
```

in MySQL Workbench.

---

## Usage

1. Start the Streamlit application:

```bash
streamlit run main.py
```

2. Open the application in your browser
3. Enter questions related to inventory or sales
4. View results generated from the MySQL database

---

## Sample Questions

* How many total T-shirts are available in stock?
* How many Nike T-shirts are available in XS size and white color?
* What is the total inventory value of all small-size T-shirts?
* How much revenue will be generated if all small-size Adidas T-shirts are sold after discounts?

---

## Project Structure

* **main.py**: The main Streamlit application script
* **langchain_helper.py**: Contains all the LangChain-related code
* **requirements.txt**: Lists the required Python packages for the project
* **few_shots.py**: Contains few-shot prompt examples
* **.env**: Configuration file for storing the Google API key

