# 🤖 RAG AI Assistant with Qdrant

An AI-powered Retrieval-Augmented Generation (RAG) assistant built with **n8n**, **Google Gemini AI**, **Qdrant Vector Database**, and **Google Drive**.

The project consists of two workflows:
- **Indexing Workflow** – Automatically processes documents from Google Drive, creates embeddings, and stores them in Qdrant.
- **Chat Workflow** – Retrieves relevant information from Qdrant and generates accurate answers using Google Gemini.

---

## ✨ Features

- 📂 Automatic document ingestion from Google Drive
- ✂️ Intelligent document chunking
- 🧠 Google Gemini Embeddings
- 🗄️ Qdrant Vector Database
- 🤖 AI Agent with Retrieval-Augmented Generation (RAG)
- 💬 Natural language question answering
- ⚡ Fully automated n8n workflows

---

## 🏗️ Architecture

```
Google Drive
      │
      ▼
Download Documents
      │
      ▼
Text Chunking
      │
      ▼
Gemini Embeddings
      │
      ▼
Qdrant Vector Store
      │
      ▼
────────────────────────────────

User Question
      │
      ▼
AI Agent
      │
      ▼
Retrieve Context
      │
      ▼
Google Gemini
      │
      ▼
Final Response
```

---

## 📂 Project Structure

```
rag-ai-assistant-with-qdrant/
│
├── indexing-workflow.json
├── chat-workflow.json
├── workflow.png
└── README.md
```

---

## 🛠 Tech Stack

| Component | Purpose |
|-----------|---------|
| n8n | Workflow Automation |
| Google Gemini AI | LLM & Embeddings |
| Qdrant | Vector Database |
| Google Drive | Document Storage |
| AI Agent | Retrieval & Response Generation |

---

## 🚀 Workflow Overview

### 1. Indexing Workflow

- Monitor a Google Drive folder
- Download newly added documents
- Split documents into chunks
- Generate embeddings using Google Gemini
- Store vectors in Qdrant

---

### 2. Chat Workflow

- Receive user query
- Retrieve relevant chunks from Qdrant
- Pass retrieved context to Gemini
- Generate an accurate answer
- Return the response to the user

---

## 📸 Workflow Screenshot

> Replace the image below with your uploaded screenshot.

![Workflow](workflow.png)

---

## ⚙️ Setup Instructions

1. Import both workflow JSON files into n8n.
2. Configure your credentials:
   - Google Drive OAuth
   - Google Gemini API
   - Qdrant API
3. Create a Qdrant collection.
4. Update node credentials and collection names.
5. Activate the workflows.
6. Upload documents to Google Drive and start chatting with the AI assistant.

---

## 📌 Use Cases

- AI Knowledge Base
- Internal Company Documentation
- Customer Support Assistant
- FAQ Chatbot
- Enterprise Search
- Document Question Answering

---

## ⚠️ Note

The exported workflows contain placeholder credential references. Replace them with your own Google Drive, Google Gemini, and Qdrant credentials before running.

---

## 👨‍💻 Author

## 👨‍💻 Author
Built by **Gaurav Sharma** ([gaurav2026-gt](https://github.com/gaurav2026-gt)) as part of hands-on learning in **n8n Automation**, **LLMs**, **RAG**, and **AI Agents**.
