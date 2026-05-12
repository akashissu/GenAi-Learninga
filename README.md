<div align="center">

# GenAI Learning Lab

### My hands-on journey through LangChain, LLMs, Embeddings & Vector Databases

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)](https://www.langchain.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Hugging Face](https://img.shields.io/badge/🤗_HuggingFace-FFD21E?style=for-the-badge)](https://huggingface.co/)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)](https://ollama.com/)

![Status](https://img.shields.io/badge/status-actively_learning-brightgreen?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/akashissu/GenAi-Learninga?style=flat-square)
![Repo Size](https://img.shields.io/github/repo-size/akashissu/GenAi-Learninga?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

</div>

---

## About

> A growing collection of notebooks where I break down **Generative AI** concepts one piece at a time — from talking to LLMs, to chunking documents, to building searchable vector indexes with FAISS and Chroma.
>
> Think of it as a **lab notebook**, not a polished product. Every folder is an experiment.

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

| Module | Topic | Status |
|--------|-------|:------:|
| `1.1-OpenAi` | Talking to OpenAI models via LangChain | Pending |
| `1.2-Ollam`  | Local LLMs with Ollama | Pending |

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
| `huggingface.ipynb` | Using HF models & `sentence-transformers` inside LangChain |

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
- OpenAI GPT
- Ollama (local)
- Hugging Face

</td>
<td valign="top" width="33%">

### Embeddings
- `text-embedding-3-small`
- `sentence-transformers`
- Ollama embeddings

</td>
<td valign="top" width="33%">

### Vector Stores
- FAISS
- ChromaDB

</td>
</tr>
<tr>
<td valign="top">

### Loaders
- `pypdf` / `pymupdf`
- `bs4` (web)
- `arxiv`
- `wikipedia`

</td>
<td valign="top">

### Splitters
- Recursive Character
- Character
- Token-based

</td>
<td valign="top">

### Tooling
- Jupyter
- python-dotenv
- ipykernel

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
| `GROQ_API_KEY` | Groq inference | Optional |
| `HF_TOKEN` | Gated Hugging Face models | Optional |
| `LANGCHAIN_API_KEY` | LangSmith tracing | Optional |

> [!WARNING]
> Never commit your `.env` file. It's already in `.gitignore` — keep it that way.

---

## Progress Tracker

- [x] Project scaffolding & environment setup
- [x] Data ingestion (PDF, web, Arxiv, Wikipedia)
- [x] Text splitting strategies
- [x] OpenAI & Ollama embeddings
- [x] FAISS vector store
- [x] ChromaDB vector store
- [ ] End-to-end RAG pipeline
- [ ] Conversational memory
- [ ] Agents & tool calling
- [ ] LangGraph workflows
- [ ] Deploying with FastAPI

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
