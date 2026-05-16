<div align="center">

# GenAI Learning Lab

### My hands-on journey through LangChain, LLMs, Embeddings & Vector Databases

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)](https://www.langchain.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Hugging Face](https://img.shields.io/badge/🤗_HuggingFace-FFD21E?style=for-the-badge)](https://huggingface.co/)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge)](https://groq.com/)
[![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)](https://ollama.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)

![Status](https://img.shields.io/badge/status-actively_learning-brightgreen?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/akashissu/GenAi-Learninga?style=flat-square)
![Repo Size](https://img.shields.io/github/repo-size/akashissu/GenAi-Learninga?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

</div>

---

## About

> A growing collection of notebooks and scripts where I break down **Generative AI** concepts one piece at a time — from talking to LLMs, to chunking documents, to building searchable vector indexes with FAISS and Chroma, and exposing chains over HTTP with LangServe.
>
> Think of it as a **lab notebook**, not a polished product. Every folder is an experiment.

---

## Project Structure

```
Langchain/
├── .env.example
├── requirements.txt
└── 1-Langchain/
    ├── 1.1-OpenAi/
    │   ├── GettingStarted.ipynb      # ChatOpenAI, invoke/stream, LangSmith tracing
    │   └── SimpleGenAi.ipynb         # Deeper OpenAI + LangChain workflows
    ├── 1.2-Ollam/
    │   └── app.py                    # Placeholder (local Ollama app — WIP)
    ├── 1.3-Groq/
    │   ├── getStarted.ipynb          # ChatGroq basics
    │   └── serve.py                  # FastAPI + LangServe translation chain
    ├── 3.2-Dataingetion/
    │   ├── 3.2-Dataingetion.ipynb    # PDF, web, Arxiv, Wikipedia loaders
    │   ├── 3.3-textspillter.ipynb    # Recursive character text splitter
    │   └── 3.4-characterSpilitter.ipynb
    ├── 3.4-embedding/
    │   ├── embedding.ipynb           # OpenAI embeddings
    │   └── ollama-embedding.ipynb    # Local embeddings via Ollama
    ├── 4.1-HuggingFace/
    │   └── huggingface.ipynb         # HF models & sentence-transformers
    └── 5-VectorDB/
        ├── 5.1-FaissDB.ipynb         # FAISS index build & query
        ├── 5.2-chromadb.ipynb        # ChromaDB persistent store
        └── speech.txt                # Sample text for vector demos
```

---

## Roadmap

```mermaid
flowchart LR
    A[LLM Basics] --> B[Data Ingestion]
    B --> C[Text Splitters]
    C --> D[Embeddings]
    D --> E[Vector DBs]
    E --> F[RAG Pipelines]
    F --> G[Agents & Tools]

    style A fill:#FFD21E,stroke:#333,color:#000
    style D fill:#412991,stroke:#333,color:#fff
    style E fill:#1C3C3C,stroke:#333,color:#fff
    style F fill:#10B981,stroke:#333,color:#fff
    style G fill:#EF4444,stroke:#333,color:#fff
```

---

## What's Inside

<details open>
<summary><b>1 · LangChain Fundamentals</b></summary>

| Path | Topic | Status |
|------|-------|:------:|
| `1.1-OpenAi/GettingStarted.ipynb` | `ChatOpenAI`, invoke/stream, LangSmith tracing | Done |
| `1.1-OpenAi/SimpleGenAi.ipynb` | OpenAI + LangChain patterns | Done |
| `1.2-Ollam/app.py` | Local LLMs with Ollama (Streamlit) | WIP |
| `1.3-Groq/getStarted.ipynb` | `ChatGroq` setup & prompts | Done |
| `1.3-Groq/serve.py` | FastAPI + LangServe hosted chain | Done |

</details>

<details open>
<summary><b>3 · Data Ingestion & Chunking</b></summary>

| Notebook | Covers |
|----------|--------|
| `3.2-Dataingetion.ipynb` | Loading PDFs, web pages, Arxiv, Wikipedia |
| `3.3-textspillter.ipynb` | Recursive character text splitter |
| `3.4-characterSpilitter.ipynb` | Character-level splitting strategies |

</details>

<details open>
<summary><b>3.4 · Embeddings</b></summary>

| Notebook | Covers |
|----------|--------|
| `embedding.ipynb` | OpenAI embeddings |
| `ollama-embedding.ipynb` | Local embeddings via Ollama |

</details>

<details open>
<summary><b>4 · Hugging Face Integration</b></summary>

| Notebook | Covers |
|----------|--------|
| `huggingface.ipynb` | HF models & `sentence-transformers` inside LangChain |

</details>

<details open>
<summary><b>5 · Vector Databases</b></summary>

| Notebook | Covers |
|----------|--------|
| `5.1-FaissDB.ipynb` | Building & querying a FAISS index |
| `5.2-chromadb.ipynb` | Persistent storage with ChromaDB |

</details>

---

## Tech Stack

<table>
<tr>
<td valign="top" width="33%">

### LLMs
- OpenAI GPT (`langchain-openai`)
- Groq (`langchain-groq`)
- Ollama (local)
- Hugging Face (`langchain-huggingface`)

</td>
<td valign="top" width="33%">

### Embeddings
- `text-embedding-3-small`
- `sentence-transformers`
- Ollama embeddings

</td>
<td valign="top" width="33%">

### Vector Stores
- FAISS (`faiss-cpu`)
- ChromaDB (`langchain-chroma`)

</td>
</tr>
<tr>
<td valign="top">

### Loaders
- `pypdf` / `pymupdf`
- `beautifulsoup4` (web)
- `arxiv`
- `wikipedia`

</td>
<td valign="top">

### Splitters
- Recursive Character (`langchain-text-splitters`)
- Character
- Token-based

</td>
<td valign="top">

### Serving & Tooling
- FastAPI + Uvicorn
- LangServe
- Streamlit (planned for Ollama UI)
- Jupyter, python-dotenv, ipykernel

</td>
</tr>
</table>

---

## Quick Start

```bash
# 1. Clone
git clone https://github.com/akashissu/GenAi-Learninga.git
cd GenAi-Learninga

# 2. Create virtual environment
python -m venv .venv
source .venv/bin/activate          # macOS / Linux
# .venv\Scripts\activate           # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Configure secrets
cp .env.example .env
# then open .env and add your API keys

# 5. Launch Jupyter
jupyter notebook
```

### Run the Groq LangServe API

```bash
cd 1-Langchain/1.3-Groq
python serve.py
# API docs: http://127.0.0.1:8000/docs
# Chain playground: http://127.0.0.1:8000/chain/playground/
```

> [!TIP]
> Running locally with **Ollama**? Install it from [ollama.com](https://ollama.com) and pull a model first:
> ```bash
> ollama pull llama3
> ollama pull nomic-embed-text
> ```

---

## Required Environment Variables

| Variable | Used for | Required |
|----------|----------|:--------:|
| `OPENAI_API_KEY` | OpenAI LLMs & embeddings | If using OpenAI |
| `GROQ_API_KEY` | Groq inference (`1.3-Groq`) | If using Groq |
| `HF_TOKEN` | Gated Hugging Face models | Optional |
| `LANGCHAIN_API_KEY` / `LANGSMITH_API_KEY` | LangSmith tracing | Optional |
| `LANGCHAIN_TRACING_V2` | Enable tracing | Optional |
| `LANGCHAIN_PROJECT` | LangSmith project name | Optional |

> [!WARNING]
> Never commit your `.env` file. It's already in `.gitignore` — keep it that way. Clear notebook cell outputs before pushing if they contain keys or secrets.

---

## Progress Tracker

- [x] Project scaffolding & environment setup
- [x] OpenAI basics (`GettingStarted`, `SimpleGenAi`)
- [x] Groq basics + LangServe API (`getStarted`, `serve.py`)
- [x] Data ingestion (PDF, web, Arxiv, Wikipedia)
- [x] Text splitting strategies
- [x] OpenAI & Ollama embeddings
- [x] Hugging Face / sentence-transformers
- [x] FAISS vector store
- [x] ChromaDB vector store
- [ ] Ollama Streamlit app (`1.2-Ollam/app.py`)
- [ ] End-to-end RAG pipeline
- [ ] Conversational memory
- [ ] Agents & tool calling
- [ ] LangGraph workflows

---

## Connect

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-akashissu-181717?style=for-the-badge&logo=github)](https://github.com/akashissu)

⭐ **Star this repo if it helps you learn too!**

</div>

---

<div align="center">
<sub>Built with curiosity, caffeine, and the occasional <code>pip install</code> regret.</sub>
</div>
