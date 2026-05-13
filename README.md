# Math RAG Pipeline with Gradio UI

A Retrieval-Augmented Generation (RAG) application built on a mathematics textbook using embeddings, vector search, and a Gradio interface for interactive question answering.

---

# Features

* PDF-based mathematical knowledge retrieval
* Text chunking and embedding generation
* Vector database integration
* Semantic search for relevant context retrieval
* RAG pipeline for accurate responses
* Interactive Gradio web interface
* Environment variable support for API keys
* Clean and modular backend structure

---

# Tech Stack

* Python
* Gradio
* LangChain
* OpenAI API
* FAISS / ChromaDB (depending on your implementation)
* Sentence Transformers / OpenAI Embeddings
* Google Colab

---

# Project Workflow

## 1. Load PDF

The mathematics textbook PDF is loaded and processed.

## 2. Text Chunking

The extracted text is divided into smaller chunks for efficient retrieval.

## 3. Embedding Generation

Embeddings are generated for all chunks using an embedding model.

## 4. Vector Database Storage

The embeddings are stored inside a vector database.

## 5. User Query

The user enters a mathematical question through the Gradio interface.

## 6. Semantic Retrieval

Relevant chunks are retrieved from the vector database.

## 7. Response Generation

The retrieved context is passed to the language model to generate the final response.

---

# Folder Structure

```bash
project/
│
├── data/
│   └── maths_book.pdf
│
├── vectorstore/
│
├── app.py
├── rag_pipeline.py
├── requirements.txt
├── README.md
└── .env
```

---

# Installation

## Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

---

# Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Mac/Linux

```bash
source venv/bin/activate
```

---

# Install Dependencies

```bash
pip install -r requirements.txt
```

---

# API Key Setup

Create a `.env` file:

```env
OPENAI_API_KEY=your_api_key_here
```

Or use Google Colab Secrets:

```python
import os
from google.colab import userdata

os.environ["OPENAI_API_KEY"] = userdata.get("OPENAI_API_KEY")
```

---

# Run the Application

```bash
python app.py
```

The Gradio interface will launch locally.

---

# Example Questions

* What is the chain rule?
* Explain Taylor series.
* What is differentiation?
* Define integration.
* Explain limits in calculus.
* What is the difference between derivatives and differentials?

---

# Future Improvements

* Add chat history memory
* Improve mathematical notation rendering
* Add OCR support for scanned PDFs
* Multi-PDF support
* Hybrid search
* Better retrieval ranking
* Deploy using Hugging Face Spaces or Streamlit Cloud

---

# Screenshots

Add screenshots of:

* Gradio UI
* Retrieval process
* Response generation
* Vector database creation

---

# Learning Outcomes

This project helped in understanding:

* Retrieval-Augmented Generation (RAG)
* Embeddings and semantic search
* Vector databases
* Prompt engineering
* Document chunking
* LLM application development
* Building AI interfaces using Gradio

---

# License

This project is for educational and learning purposes.

---

# Author

Hooria Khan
