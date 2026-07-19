# RepoSense AI - Agentic GitHub Repository Assistant

RepoSense AI is an **Agentic AI** project that helps users understand any public GitHub repository by simply asking questions in natural language. It uses a **ReAct AI Agent**, **FAISS**, **Sentence Transformers**, and **Groq Llama 3.1** to search the repository, choose the required tools automatically, and generate answers based only on the repository content.

---

## Features

- Analyze any public GitHub repository.
- Ask questions in natural language.
- Automatically choose the required tools to answer the question.
- Perform semantic search using FAISS.
- Explain source code files.
- Summarize the repository and README.
- Find relevant files related to a query.

---

## Workflow

1. Clone the GitHub repository.
2. Read source code and documentation files.
3. Split files into smaller chunks.
4. Generate embeddings using Sentence Transformers.
5. Store embeddings in a FAISS vector database.
6. Convert repository functions into AI tools.
7. Create a ReAct Agent with access to these tools.
8. User asks a question in natural language.
9. The agent decides which tool(s) to use.
10. The agent retrieves the required information.
11. Groq Llama generates the final answer.

---

## Technologies Used

- Python
- LangChain
- LangGraph
- Groq API
- Llama 3.1 8B Instant
- Sentence Transformers
- FAISS
- GitPython
- NumPy

---

## AI Techniques Used

### Agentic AI

- ReAct Agent
- Tool Calling
- Multi-step Reasoning
- Autonomous Tool Selection

### Retrieval-Augmented Generation (RAG)

- Sentence Transformer Embeddings
- FAISS Vector Search
- Semantic Search
- Context-Aware Answer Generation

---

## Available Tools

| Tool | Purpose |
|------|---------|
| Search Repository | Searches the repository for relevant code |
| Explain File | Explains a specific file |
| Find Relevant Files | Finds files related to a query |
| Summarize Repository | Gives an overview of the repository |
| Summarize README | Summarizes the README file |
| Folder Structure Overview | Explains the project structure |

---

## Example Agent Workflow

**User Question**

```text
How is authentication implemented?
```

**Agent Process**

```text
Thought
↓

Search Repository

↓

Find Relevant Files

↓

Explain File

↓

Final Answer
```

The user only asks a question. The AI agent automatically decides which tools to use and combines their results to generate the answer.

---

## Repository Structure

```text
RepoSense-AI/
│
├── notebooks/
│   └── RepoSense_AI_Agent.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## How to Run

```bash
git clone <repository-url>
cd RepoSense-AI
pip install -r requirements.txt
```

Open the notebook in **Google Colab** or **Jupyter Notebook** and run all cells.

When prompted:

1. Enter your Groq API Key.
2. Enter a public GitHub repository URL.
3. Ask questions about the repository.

---

## Example Questions

```text
Explain this repository.

How does authentication work?

Summarize the README.

Which files are most important?

How is computer vision used?

Explain the project architecture.
```

---

## Future Improvements

- Support private GitHub repositories.
- Analyze GitHub Issues and Pull Requests.
- Add a Streamlit web interface.
- Support multiple AI agents.
- Improve code explanation quality.

---

## Author

~ Avni Goel
