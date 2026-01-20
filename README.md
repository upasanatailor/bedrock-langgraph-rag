# 🚀 Agentic RAG: Multi-Format Document Intelligence

An enterprise-grade **Retrieval-Augmented Generation (RAG)** system designed to analyze PDFs, Markdown, and JSON files. This project leverages **LangGraph** for stateful orchestration and **Amazon Bedrock** for high-reasoning inference, providing a robust "Chat-with-your-Data" experience.



## 🛠️ Tech Stack
* **Orchestration:** LangGraph, LangChain
* **AI Models:** Amazon Bedrock (Nova-Lite, Claude 3.5, Titan V2)
* **Vector Store:** ChromaDB
* **Environment:** Python 3.9+, Jupyter Notebook
* **Package Management:** `uv` (by Astral)

---

## ⚡ Quick Start with `uv`

This project uses **[uv](https://github.com/astral-sh/uv)** for ultra-fast dependency management. You do not need to install packages one by one; `uv` handles the entire `requirements.txt` in seconds.

### 1. Install `uv`
If you don't have `uv` installed yet:

**macOS/Linux:**
```bash
curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
Windows (PowerShell):

Bash

powershell -c "irm [https://astral.sh/uv/install.ps1](https://astral.sh/uv/install.ps1) | iex"
2. Setup Environment & Install Dependencies
Run these commands in the project root to create a virtual environment and sync all libraries from requirements.txt automatically:

Bash

# Create a virtual environment
uv venv

# Activate the environment
# On macOS/Linux:
source .venv/bin/activate
# On Windows:
.venv\Scripts\activate

# Install all packages from requirements.txt at once
uv pip install -r requirements.txt
📂 Project Structure
*.ipynb: Jupyter Notebooks containing the RAG logic and experimentation.

chroma_db/: Persistent local vector database storage.

requirements.txt: List of dependencies (LangChain, Bedrock, etc.).

.env: (User-created) Stores AWS credentials and configuration.

🧪 Development Workflow
Experimentation: Initial RAG parameters (chunk size, overlap, and prompt templates) were tuned in Jupyter Notebooks for rapid iteration.

Management: Used uv to maintain a lightning-fast, reproducible development environment.

Inference: Integrated Amazon Nova-Lite via the Bedrock Converse API for optimized response times and cost efficiency.

🚀 Usage
After installing dependencies, launch the notebook to interact with the RAG pipeline:

Bash

uv run jupyter notebook
📝 Configuration (.env)
Create a .env file in the root directory to securely manage your AWS access:

Code snippet

AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
AWS_REGION=eu-central-1
🌟 Project by Upasana Tailor
Focused on building stateful, agentic AI solutions.


---

### 📥 How to "Download" it:
1.  Click the **Copy** icon at the top right of the code block above.
2.  Open any text editor (Notepad, VS Code, TextEdit).
3.  Paste the content.
4.  Save the file as **`README.md`** in your project folder.

[Adding and updating documents in Chroma with LangChain](https://www.youtube.com/watch?v=GONbsWzP3SY)

This video is relevant because it shows how to effectively manage document ingestion and metadata within ChromaDB, which is a key part of the technical workflow described in your README.
