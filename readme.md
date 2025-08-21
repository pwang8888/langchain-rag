# 🧠 LangChain RAG: Question Answering with Local Documents

This project builds a simple Retrieval-Augmented Generation (RAG) system using LangChain, ChromaDB, and OpenAI. It lets you ask questions about your own documents using AI.

---

## 📦 Features

- Load documents using `unstructured` via LangChain's `DirectoryLoader`
- Create a local vector database with `ChromaDB`
- Use OpenAI embeddings for semantic search
- Query your documents with LangChain

---

## 🚀 Installation

### 1. Clone the repo

```bash
git clone git@github.com:pwang8888/langchain-rag.git
cd langchain-rag
```

### 2. Install dependencies

**MacOS users:**

```bash
conda install onnxruntime -c conda-forge
```

**Windows users:**

Install [Microsoft C++ Build Tools](https://github.com/bycloudai/InstallVSBuildToolsWindows?tab=readme-ov-file)

Then install Python packages:

```bash
pip install -r requirements.txt
pip install "unstructured[md]"
```

---

## 🔐 Set up OpenAI API key

Create a `.env` file with:

```env
OPENAI_API_KEY=your_openai_key
```

---

## 🏗️ Usage

### Step 1: Create the database

```bash
python create_database.py
```

### Step 2: Ask a question

```bash
python query_data.py "How does Alice meet the Mad Hatter?"
```


## 📝 Requirements

See `requirements.txt` for full package list.
