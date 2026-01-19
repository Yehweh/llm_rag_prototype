# LLM-based RAG Prototype

This repository contains a simple end-to-end **Retrieval-Augmented Generation (RAG)** prototype built to understand how document-based question answering systems work using Large Language Models.

The focus of this project is **learning and system understanding**, not production-scale optimization.

---

## What this project does

- Ingests documents and splits them into chunks  
- Creates vector embeddings for efficient retrieval  
- Retrieves relevant context based on a user query  
- Passes retrieved context to an LLM to generate answers  

This helps reduce hallucinations by grounding responses in source documents.

---

## Why this project exists

This project was built as a **learning prototype** to:
- Understand the full RAG pipeline end-to-end  
- Explore prompt structuring and context injection  
- Learn trade-offs related to context size, latency, and response quality  

It is **not intended to be production-ready**.

---

## Project structure

create_database.py # Ingests documents and builds the vector store
query_data.py # Queries the vector store and generates responses
compare_embeddings.py # (Optional) Used to experiment with embeddings
requirements.txt
README.md

## How to run locally

1. Create and activate a virtual environment  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

Run the database creation script:

python create_database.py


Query the system:

python query_data.py

Current status

Early-stage prototype

Built for experimentation and learning

Actively open to improvements and refactoring