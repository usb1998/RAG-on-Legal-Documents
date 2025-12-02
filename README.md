# Legal Document Question Answering using Retrieval-Augmented Generation (RAG)

This project implements an end-to-end **Retrieval-Augmented Generation (RAG)** pipeline for **legal document question answering**.  
The system is designed to retrieve legally relevant clauses and generate accurate answers grounded in the source documents.

The project includes:
- Data preprocessing  
- Chunking of legal documents  
- MPNet-based semantic retrieval  
- Cross-encoder reranking for improved relevance  
- Extractive answer generation  
- ROUGE/BLEU evaluation of model performance  

---

## 🚀 Project Overview

Legal documents require precise clause-level extraction rather than free-form text generation.  
This RAG pipeline is optimized for **high recall and faithful extraction** using:

- **all-mpnet-base-v2** for embedding-based retrieval  
- **cross-encoder/ms-marco-MiniLM-L-6-v2** for reranking retrieved chunks  
- **extractive answer selection** instead of generative LLMs  
- Improved chunking (`600` size, `150` overlap) to preserve legal clause structure  

This ensures the system produces answers that are **factual, grounded, and legally accurate**.

---

