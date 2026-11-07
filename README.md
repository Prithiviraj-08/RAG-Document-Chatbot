# RAG Document Chatbot

A beginner-friendly **Retrieval-Augmented Generation (RAG)** application built with Python.

Upload a PDF document, ask questions about its content, and get answers grounded in the uploaded document.

## Features

- Upload a PDF document
- Extract text using `pypdf`
- Split document text into overlapping chunks
- Generate embeddings using Sentence Transformers
- Store and search embeddings with FAISS
- Retrieve the most relevant document sections for each question
- Generate grounded answers using Groq
- Chat-style interface using Streamlit
- Maintain conversation history with Streamlit session state
- Clear chat history when a different PDF is uploaded
- Handle PDFs with no readable text
- Handle missing API keys and model/API errors
- Avoid answering from outside the uploaded document

## Tech Stack

- Python
- Streamlit
- pypdf
- Sentence Transformers
- FAISS
- Groq
- python-dotenv

## How RAG Works in This Project

```text
PDF Upload
    ↓
Text Extraction
    ↓
Text Chunking
    ↓
Document Embeddings
    ↓
FAISS Vector Index
    ↓
User Question
    ↓
Question Embedding
    ↓
Similarity Search
    ↓
Relevant Document Chunks
    ↓
Groq LLM
    ↓
Grounded Answer
```

