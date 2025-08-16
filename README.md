# 📄 DocuVerse AI - an LLMOps Project 🚀

An end-to-end LLMOps-powered Document Intelligence Platform that enables users to interact with documents like never before. From semantic understanding to side-by-side comparison and intelligent querying — all deployed and automated using modern CI/CD practices on AWS.

'''

## ✨ Features

### 🔍 Document Analysis

Automatically extract, summarize, and interpret content from uploaded documents using LLM + RAG pipeline.

### 🆚 Compare Two Documents

Upload any two documents and get a structured comparison.

### 💬 Talk with a Single Document

Ask questions and get accurate answers from a single document using Retrieval-Augmented Generation (RAG).

### 📚 Talk with Multiple Documents

Query across multiple related documents and get consolidated insights using intelligent chunking and vector search.

### ⚙️ CI/CD Pipeline

Fully automated Dev → Test → Deploy pipeline with version control, testing, linting, and push-to-AWS integration.

### ☁️ AWS Deployment

Scalable and secure deployment using AWS services such as S3, EC2, Lambda, and API Gateway.

'''

## 🧠 Tech Stack
1. Layer	        Tech
2. Language	        Python 🐍
3. LLM Framework	LangChain
4. RAG Pipeline	    Hugging Face Embeddings + FAISS/ChromaDB
5. LLMs Used	    OpenAI, Ollama, or any custom endpoint
6. Frontend	        Streamlit / FastAPI
7. CI/CD	        GitHub Actions + AWS CodePipeline
8. Deployment	    AWS EC2 / S3 / Lambda
9. Storage	        S3 (for documents), Vector DB for embeddings

'''

## Minimum Requirements

1. LLM Model - groq, openai, gemini, huggingface, claude, etc

2. Embedding Model - huggingface, openai, gemini

3. Vector DB - inmemory, persistent, cloude-based

'''

## 📂 Project Structure

```plaintext
DOCUMENT_PORTAL/
│
├── config/                    # Configuration files
│   └── config.yaml            # Main app configuration
│
├── env/                       # Environment-related logic (if any)
│
├── exception/                 # Custom exception classes
│   └── custom_exception.py
│
├── logging/                   # Logging setup and formatters
│
├── notebook/                  # Jupyter experiments / test notebooks
│   └── experiments.ipynb
│
├── prompt_lib/                # Prompt templates and prompt builders
│
├── src/                       # Core application logic
│   ├── doc_analyser/          # Modules for document content analysis
│   ├── doc_compare/           # Logic for side-by-side document comparison
│   ├── multidoc_chat/         # Querying across multiple documents
│   └── singledoc_chat/        # Interacting with a single document
│
├── static/                    # Static assets (if using Streamlit/FastAPI web UI)
│
├── templates/                 # HTML templates for web rendering
│
├── utils/                     # Helper utilities (S3 uploaders, embedding handlers, etc.)
│
├── .env                       # Local env vars (dev only – API keys are managed via AWS Secrets Manager)
├── app.py                     # Main app entrypoint (FastAPI or CLI)
├── streamlit_ui.py            # Streamlit-based user interface
├── requirements.txt           # Python dependencies
├── setup.py                   # Package/module setup file
└── README.md                  # 📘 You’re here!

```

## 🚀 How It Works
- Upload Documents — via UI or API.

- Text Extraction — from PDF, DOCX, PPTX, etc.

- Embedding + Storage — chunks are embedded and stored in Vector DB.

- RAG-Powered Responses — using LangChain + LLMs.

- Compare or Chat — depending on selected mode.

- CI/CD Pipeline — triggers auto-deploy to AWS on each commit.
