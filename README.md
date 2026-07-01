# RAG Implementation with PDF and Direct Documents

## Overview

This project implements a Retrieval-Augmented Generation (RAG) pipeline that supports both **PDF documents** and **directly provided text documents**. It extracts or accepts text, generates vector embeddings using Sentence Transformers, stores them in a FAISS vector database, and retrieves the most relevant content based on semantic similarity. The retrieved context is then passed to an LLM to generate accurate and context-aware responses.

## Features

* Load and process PDF documents
* (Also) Use direct text documents provided in the code
* Text chunking for efficient retrieval
* Generate embeddings using Sentence Transformers
* Store embeddings in FAISS vector database
* Fast semantic similarity search
* Context-aware question answering using an LLM

## Tech Stack

* Python
* PyPDF
* Sentence Transformers
* FAISS
* LangChain
* NumPy

## Project Workflow

1. Load a PDF file or provide text documents directly in the code.
2. Extract and preprocess the text.
3. Split text into chunks (if required).
4. Generate embeddings for each document or chunk.
5. Store embeddings in the FAISS vector database.
6. Retrieve the most relevant content based on the user query.
7. Generate the final answer using an LLM.

## Example of Direct Documents

```python
documents = [
    "RAG stands for Retrieval Augmented Generation.",
    "Embeddings convert text into vectors.",
    "FAISS is used for similarity search.",
    "Chunking splits large documents into smaller pieces."
]
```

## Installation

```bash
pip install pypdf sentence-transformers faiss-cpu langchain numpy
```

## Author

Developed as a hands-on project demonstrating Retrieval-Augmented Generation (RAG) using PDF documents, direct text documents, semantic search, Sentence Transformers, and FAISS vector indexing.
