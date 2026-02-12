Simple RAG Pipeline with LangChain & Ollama

A lightweight Retrieval-Augmented Generation (RAG) project demonstrating how to combine semantic search with a Large Language Model (LLM) for context-aware question answering.

This project uses LangChain, FAISS, and Ollama to load documents, split them into chunks, generate embeddings, and retrieve relevant context before passing it to an LLM.

---

Overview

Traditional LLMs rely only on their training data.  
RAG (Retrieval-Augmented Generation) enhances responses by retrieving relevant external knowledge and injecting it into the prompt.

This repository showcases:

- Document ingestion
- Text chunking
- Embedding generation
- Vector similarity search (FAISS)
- Contextual Q&A using an LLM

---

Features

- Document loading from web sources  
- Text chunking using RecursiveCharacterTextSplitter  
- Embeddings via Ollama (nomic-embed-text)  
- Vector storage & retrieval with FAISS  
- LLM responses using Ollama (llama2)  
- End-to-end RAG workflow  

---

Tech Stack

- LangChain – Orchestration framework
- FAISS – Vector similarity search
- Ollama – Local LLM & embeddings
- Python – Core language

---

Architecture

User Query  
→ Embed Query  
→ FAISS Similarity Search  
→ Retrieve Relevant Chunks  
→ Augment Prompt with Context  
→ LLM Response  

---

Workflow

1. Load Documents  
   WebBaseLoader fetches content

2. Split Text  
   RecursiveCharacterTextSplitter creates chunks

3. Generate Embeddings  
   Ollama embedding model

4. Store Vectors  
   FAISS vector database

5. Query  
   Retrieve relevant chunks  
   Pass context to LLM

---

Installation

1. Clone Repository
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
