# Potterverse Pathfinder RAG

A multi-document Retrieval-Augmented Generation system that answers questions from the Harry Potter book series using LangChain, Hugging Face language models, Sentence-BERT embeddings, and FAISS vector search.

## Project Overview

Potterverse Pathfinder is a semantic search and question-answering application designed to retrieve relevant passages from multiple documents and generate context-aware responses.

The system processes the seven Harry Potter books, splits the text into manageable chunks, converts the chunks into vector embeddings, stores them in a FAISS vector database, and retrieves the most relevant passages for each user query.

The retrieved context is then passed to a large language model to generate a concise answer with source references.

## Key Features

- Multi-document question answering
- Retrieval-Augmented Generation pipeline
- Semantic search using sentence embeddings
- FAISS-based vector similarity search
- LangChain RetrievalQA integration
- Hugging Face language model support
- Source document and page references
- Configurable chunk size and retrieval parameters
- Support for conversational and context-aware responses

## System Architecture

```text
Harry Potter PDF Documents
            |
            v
      PDF Text Extraction
            |
            v
 Recursive Text Chunking
            |
            v
 Sentence-BERT Embeddings
            |
            v
      FAISS Vector Store
            |
            v
     Similarity Retrieval
            |
            v
 Retrieved Context + Query
            |
            v
   Hugging Face Language Model
            |
            v
 Answer with Source References
