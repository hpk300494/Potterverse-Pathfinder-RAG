                    User Question
                          │
                          ▼
                  LangChain RetrievalQA
                          │
        ┌─────────────────┴─────────────────┐
        ▼                                   ▼
Sentence-BERT Embeddings              HuggingFace LLM
        │                                   ▲
        ▼                                   │
      FAISS Vector Store ◄──── Retrieved Context
        ▲
        │
 Harry Potter PDF Documents
