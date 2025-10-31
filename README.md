# 🤖 Agentic AI Frameworks & Fundamentals  
*A hybrid, intelligent agentic AI system combining Gemini, LangChain, FAISS & Tavily for reasoning, retrieval, and automation.*

[![Open in Colab](https://colab.research.google.com/drive/1KLL9B85krXibcgNWBJ5-dmarBWPZ2LJ0?usp=sharing) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🧠 Project Overview  

**Agentic AI Frameworks & Fundamentals** is an advanced AI system built to demonstrate how multiple intelligent components can collaborate to perform real-world reasoning and decision-making tasks.  

This project integrates:  
- **Google Gemini (Generative AI)** → the reasoning and language generation engine.  
- **LangChain** → the orchestration framework connecting memory, tools, and model logic.  
- **FAISS** → a vector-based retrieval system for knowledge grounding.  
- **Tavily** → a real-time web search API that extends the agent’s intelligence with up-to-date information.  

Together, these modules enable an AI agent to:  
✅ Retrieve information from local document databases (FAISS).  
✅ Search the live internet when local data isn’t sufficient (Tavily).  
✅ Reason step-by-step using the ReAct framework.  
✅ Analyze text, summarize documents, check facts, and classify sentiment.  
✅ Generate structured, context-aware responses automatically.  

---

## 🧩 Core Features  

### 🧠 1. **Retrieval-Augmented Reasoning (RAG)**
- Hybrid retrieval pipeline: local FAISS + Tavily web search.  
- Contextual question answering: answers backed by internal documents or verified online data.  
- Adaptive fallback mechanism — if FAISS retrieval fails, Tavily search is triggered.

### 🕵️ 2. **Fact-Checking Agent**
- Fetches live evidence using Tavily API.  
- Uses Gemini to analyze claim accuracy and returns verdicts: `TRUE`, `FALSE`, `PARTIALLY TRUE`, or `UNVERIFIED`.  
- Provides confidence level and key supporting evidence.  

### 💬 3. **Product Review Analyst**
- Summarizes customer reviews in 3 lines.  
- Extracts positives, negatives, and emotional tone.  
- Detects overall sentiment (positive / negative / neutral).  
- Auto-generates thank-you or apology emails accordingly.

### 📄 4. **Summarization with Retry**
- Gemini-based summarizer with exponential backoff retry logic.  
- Handles API rate limits gracefully.  
- Ensures reliable results even under heavy load.  

### ✂️ 5. **Chunking and Overlap Handling**
- Breaks large documents into smaller overlapping chunks for embedding.  
- Maintains sentence continuity and contextual flow.  

### 💬 6. **Interactive Question Answering**
- Responds intelligently to user queries.  
- Uses internal documents first → switches to Tavily search if context missing.  
- Explains answers clearly, showing which source (internal or internet) was used.

---

## ⚙️ Tech Stack  

| Layer | Technology | Purpose |
|-------|-------------|----------|
| 🧠 **LLM Engine** | Google Gemini 2.0 Flash | Core reasoning, generation, summarization |
| 🔗 **Framework** | LangChain | Tool integration, memory, and control flow |
| 🔍 **Vector Store** | FAISS | Document embedding & semantic search |
| 🌐 **Web Search** | Tavily | Real-time fact retrieval |
| 🤗 **Embeddings** | Hugging Face Sentence Transformers | Semantic encoding |
| 💻 **Language** | Python | Core implementation |
| 📘 **Notebook** | Jupyter | Development & experimentation |

---

## 🚀 Getting Started  

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/pm1023/Agentic_AI_Frameworks_and_Fundamentals.git
cd Agentic_AI_Frameworks_and_Fundamentals
