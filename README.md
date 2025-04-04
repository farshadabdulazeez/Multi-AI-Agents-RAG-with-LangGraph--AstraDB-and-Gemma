# 🤖 Multi-Agent RAG System with LangGraph, AstraDB, and Gemma

This project implements a **Multi-Agent Retrieval-Augmented Generation (RAG) system** using:

- 🧠 **LangGraph** – to orchestrate intelligent multi-agent workflows  
- 🌐 **Wikipedia Search** – for public knowledge retrieval  
- 🔍 **AstraDB** – as a scalable vector store for custom document embedding retrieval  
- ✨ **Gemma** – for enhanced natural language understanding and generation  

The system intelligently routes user queries between Wikipedia and a custom vector store using LangGraph’s agent-based architecture. This hybrid setup ensures accurate, relevant, and context-aware responses.

---

## 🚀 Features

- 🧩 **Multi-Agent Design**: Modular agents for query rephrasing, Wikipedia search, vector DB search, and response generation.
- 🔄 **Routing Logic**: Dynamically decides which path to take based on query type.
- 📚 **Context-Aware Retrieval**: Integrates both live Wikipedia data and your custom knowledge base.
- 🗃️ **AstraDB Integration**: Uses Cassandra + vector embeddings for scalable retrieval.
- 🗨️ **Gemma LLM**: Powers the reasoning and generation of final responses.
- 🔎 **Prompt Engineering**: Utilizes in-context prompting for better agent performance.

---

## 🛠️ Tech Stack

- `LangGraph`
- `Gemma` (via HuggingFace / LangChain)
- `AstraDB` (Vector Store)
- `Wikipedia API`
- `LangChain`
- `Python 3.10+`

---

## ⚙️ How It Works

1. **User inputs a question**
2. **Router agent** decides:
   - → Search Wikipedia
   - → Search AstraDB
3. **Relevant documents** are retrieved and passed to the generation agent
4. **Gemma LLM** composes the final response using retrieved knowledge

---

