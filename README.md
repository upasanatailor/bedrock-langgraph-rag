## Project

# 🚀 Agentic RAG: Multi-Format Document Intelligence

An enterprise-grade **Retrieval-Augmented Generation (RAG)** system designed to analyze **PDF**, **Markdown**, and **JSON** documents. This project leverages **LangGraph** for stateful orchestration and **Amazon Bedrock** for high-reasoning inference, enabling a powerful and scalable **Chat-with-your-Data** experience.

---

## ✨ Key Features

* 📄 Multi-format document ingestion (PDF, Markdown, JSON)
* 🧠 Agentic, stateful workflows using **LangGraph**
* 🔍 Semantic search with **ChromaDB**
* ⚡ High-performance inference via **Amazon Bedrock**
* 🧩 Modular, extensible RAG pipeline

---

## 🛠️ Tech Stack

| Category            | Tools                                            |
| ------------------- | ------------------------------------------------ |
| **Orchestration**   | LangGraph, LangChain                             |
| **AI Models**       | Amazon Bedrock (Nova-Lite, Claude 3.5, Titan V2) |
| **Vector Store**    | ChromaDB                                         |
| **Environment**     | Python 3.9+, Jupyter Notebook                    |
| **Package Manager** | `uv` (Astral)                                    |

---

## ⚡ Quick Start with `uv`

This project uses **[uv](https://github.com/astral-sh/uv)** for ultra-fast Python dependency management. It installs all dependencies from `requirements.txt` in seconds.

### 1️⃣ Install `uv`

**macOS / Linux**

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows (PowerShell)**

```powershell
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

---

### 2️⃣ Set Up Virtual Environment & Install Dependencies

Run the following commands from the project root:

```bash
# Create a virtual environment
uv venv

# Activate the environment
# macOS / Linux
source .venv/bin/activate

# Windows
.venv\Scripts\activate

# Install all dependencies
uv pip install -r requirements.txt
```

---

## 📂 Project Structure

```text
.
├── *.ipynb           # Jupyter notebooks for RAG logic & experiments
├── chroma_db/        # Persistent ChromaDB vector store
├── requirements.txt  # Python dependencies
├── .env              # AWS credentials & configuration (user-created)
└── README.md
```

---

## 🧪 Development Workflow

* **Experimentation**  
  Tuned RAG parameters such as chunk size, overlap, and prompt templates directly in Jupyter Notebooks for rapid iteration.

* **Environment Management**  
  Used `uv` to ensure a reproducible and lightning-fast development setup.

* **Inference**  
  Integrated **Amazon Nova-Lite** via the **Bedrock Converse API** to optimize latency and cost while maintaining strong reasoning performance.

---

## 🚀 Usage

After installing dependencies, launch Jupyter Notebook to interact with the RAG pipeline:

```bash
uv run jupyter notebook
```

---

## 📝 Configuration (`.env`)

Create a `.env` file in the project root to securely store your AWS credentials:

```env
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
AWS_REGION=eu-central-1
```

> ⚠️ **Never commit your `.env` file to version control.**

---

## 📚 References & Learning Resources

* ▶️ **[Adding and Updating Documents in ChromaDB with LangChain](https://www.youtube.com/watch?v=GONbsWzP3SY)**  
  This video demonstrates effective document ingestion and metadata management in ChromaDB—a core component of this project’s RAG workflow.

---

## 🌟 Author

**Upasana Tailor**  
Focused on building **stateful, agentic AI systems** for real-world enterprise use cases.

---

## 📥 Download & Use

1. Copy this repository or the contents of this file.
2. Paste into a text editor (VS Code, Notepad, etc.).
3. Save as **`README.md`** in your project root.
4. Start building with Agentic RAG 🚀
