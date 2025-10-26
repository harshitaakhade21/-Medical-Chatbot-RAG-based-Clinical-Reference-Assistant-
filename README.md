# -Medical-Chatbot-RAG-based-Clinical-Reference-Assistant-
Context-aware Q&A over a local medical knowledge base using FAISS vector search + HuggingFace or Groq-hosted LLMs.
# .

🧠 Overview
This project implements a Retrieval-Augmented Generation (RAG) pipeline that lets you ask medical questions grounded in a curated PDF knowledge base (e.g. an encyclopedia of medicine). Instead of hallucinating, the LLM is constrained by retrieved passages from a FAISS vector store built from your documents.

Two primary entry points:

connect_memory_with_llm.py – CLI prototype using a HuggingFace Inference endpoint (e.g. Mistral 7B Instruct).
medibot.py – Streamlit chat UI using a Groq-hosted model (Llama 4 Maverick) with retrieval.
