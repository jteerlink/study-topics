📚 1. Lesson Overview

🎯 Objectives:
By the end of this multi-module lesson, you’ll be able to:
	•	Manually construct each component of a RAG pipeline.
	•	Apply effective document preprocessing and chunking strategies.
	•	Compute and store vector embeddings locally.
	•	Build a semantic retriever using FAISS or Chroma with custom indexing.
	•	Integrate with a local LLM (via ollama) for context-grounded generation.
	•	Evaluate retrieval quality and handle hallucinations.

🧰 Stack:
	•	LLM: Ollama (LLaMA 3 or Mistral)
	•	Embedder: sentence-transformers → all-MiniLM-L6-v2
	•	Vector DB: FAISS (baseline), Chroma (advanced option)
	•	Preprocessing: pypdf, nltk, re
	•	No LangChain or agentic tools — we’ll use them after the manual version for contrast

⸻
Module
Topic
Outcome
1
🔍 RAG Architecture Deep Dive
Understand flow: input → retrieve → generate
2
📄 Data Ingestion & Preprocessing
Load PDFs/Markdown, clean, normalize
3
✂️ Document Chunking Strategies
Fixed, overlap, semantic
4
🔢 Embedding with Sentence Transformers
Generate dense vectors
5
🗃️ Vector Database Setup (FAISS)
Store, search, and rank results
6
🧠 LLM Integration with Ollama
Use prompt templates, local inference
7
🔁 Putting It All Together
End-to-end RAG pipeline
8
📈 Evaluation & Extension
RAGEval, hallucination handling, scaling



	•	Precision control over:
	•	how chunks are created
	•	which documents get embedded or excluded
	•	how relevance is scored and re-ranked
	•	RAG vs Fine-tuning: cost, latency, flexibility
	•	Optimizing local RAG for laptop performance
	•	Common failure modes: embedding drift, retrieval miss, hallucination
	•	Modular design: ability to swap out LLMs, retrievers, or chunkers
