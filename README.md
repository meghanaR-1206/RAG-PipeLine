# Ask Your Medical Report – RAG-Based Health Q&A System

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline that enables users to upload their personal medical reports (PDFs) and ask context-aware questions. The system parses, chunks, embeds, and retrieves relevant sections of the medical report to generate accurate answers using OpenAI's GPT.

---

##  Features

-  **RAG Pipeline**: Combines vector search and keyword retrieval for precise document chunking and retrieval.
-  **PDF Support**: Parses medical reports in PDF format using LlamaParse.
-  **Vector Search with ChromaDB**: Efficient chunk embedding and semantic retrieval.
-  **LLM Integration**: Uses OpenAI’s GPT (via LangChain) for contextual answer generation.
- **Hybrid Retrieval**: Combines BM25 and vector search using LangChain’s EnsembleRetriever.
- **Cohere Re-ranking**: Boosts result quality by reordering retrieved chunks by relevance.
- **Medical Use Cases**: Blood test interpretation, liver/cholesterol health explanations, diagnostic term insights.

---

##  Tech Stack

- **Python**
- **LangChain**
- **ChromaDB**
- **OpenAI API**
- **LlamaParse**
- **Cohere API**
- **FastEmbed**
- **Streamlit** *(optional for UI)*

##  Sample Query

PDF content: “LDL cholesterol level: 172 mg/dL (high)”

User Question: "Is 172 mg/dL of LDL cholesterol high?"

Generated Answer:
“According to your uploaded report, your LDL cholesterol level is 172 mg/dL, which falls under the high category. This may require lifestyle or medication interventions. Please consult your physician for personalized advice.”

