# PDF Chatbot using RAG

A simple AI PDF Chatbot built using **Python, Streamlit, ChromaDB, Sentence Transformers, and OpenRouter**.

## Features

* Upload and read PDF documents
* Split PDF text into chunks
* Generate text embeddings
* Store embeddings in ChromaDB
* Search relevant information from the PDF
* Generate answers using an LLM
* Simple Streamlit web interface

## Technologies

* Python
* Streamlit
* ChromaDB
* Sentence Transformers
* LangChain
* OpenRouter
* PyPDF

## Project Structure

```text
pdf-chatbot-rag-main/
│
├── app.py
├── config.py
├── requirements.txt
├── .env
│
├── data/
│   └── sample.pdf
│
├── utils/
│   ├── chunking.py
│   ├── embeddings.py
│   ├── openrouter_llm.py
│   ├── pdf_reader.py
│   ├── prompt_builder.py
│   ├── retriever.py
│   └── vector_db.py
│
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/supriyaA5/pdf-chatbot.git
```

Go to the project folder:

```bash
cd pdf-chatbot
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## API Key

Create a `.env` file and add your OpenRouter API key:

```text
OPENROUTER_API_KEY=your_api_key
```

Do not upload the `.env` file to GitHub.

## Run the Application

Start the Streamlit application:

```bash
streamlit run app.py
```

Then open the local URL shown in the terminal.

Usually:

```text
http://localhost:8501
```

## How It Works

```text
PDF
 ↓
Text Extraction
 ↓
Text Chunking
 ↓
Embeddings
 ↓
ChromaDB
 ↓
Semantic Search
 ↓
Relevant Context
 ↓
LLM
 ↓
Answer
```

## Author

**Alla Sai Supriya**

## License

This project is created for educational purposes.
