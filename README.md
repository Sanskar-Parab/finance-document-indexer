# 💰 FinMate AI – Personal Finance Manager with RAG

FinMate AI is an AI-powered Personal Finance Assistant built with **n8n** that helps users analyze bank statements, answer financial queries, track expenses, identify recurring payments, and provide personalized financial insights through **text and voice conversations**.

The repository contains **two n8n workflows**:

1. **Finance-RAG** – Automatically indexes uploaded financial documents into Pinecone.
2. **FinMate AI Assistant** – A Telegram-based AI assistant that retrieves knowledge from the indexed documents using Retrieval-Augmented Generation (RAG).

---

# 🚀 Features

- 🤖 AI-powered Personal Finance Assistant
- 📄 Automatic Bank Statement Processing
- 📂 Google Drive Document Monitoring
- 🔍 Retrieval-Augmented Generation (RAG)
- 📦 Pinecone Vector Database
- 🧠 Semantic Search
- 💬 Telegram Chatbot
- 🎙️ Voice & Text Support
- 📝 Speech-to-Text using AssemblyAI
- 🔊 AI Text-to-Speech using Groq
- 💵 Expense Analysis
- 📊 Spending Insights
- 💳 Income Tracking
- 🔁 Recurring Payment Detection
- 🎯 Savings Goal Planning
- 🧠 Conversation Memory

---

# 🛠 Tech Stack

- n8n
- Telegram Bot API
- Google Drive API
- Pinecone
- Hugging Face Embeddings
- OpenRouter
- Groq
- AssemblyAI

---

# 📂 Repository Structure

```
Finance-Rag.json
    │
    ├── Watches Google Drive
    ├── Downloads new documents
    ├── Splits text into chunks
    ├── Generates embeddings
    └── Stores vectors in Pinecone

AI Personal Finance Manager.json
    │
    ├── Telegram Bot
    ├── Voice & Text Support
    ├── Retrieves data from Pinecone
    ├── AI Financial Assistant
    └── Generates responses
```

---

# 🔄 Overall Workflow

```
          Upload Bank Statement
                   │
                   ▼
           Google Drive Folder
                   │
                   ▼
         Finance-RAG Workflow
                   │
      Download & Extract Text
                   │
                   ▼
        Recursive Text Splitter
                   │
                   ▼
      Hugging Face Embeddings
                   │
                   ▼
        Pinecone Vector Store
                   │
        ─────────────────────
                   │
                   ▼
      AI Personal Finance Manager
                   │
           Telegram Bot
         Text / Voice Input
                   │
      AssemblyAI (Speech-to-Text)
                   │
                   ▼
            FinMate AI Agent
                   │
        Retrieve Relevant Data
          from Pinecone RAG
                   │
                   ▼
      Financial Analysis & Advice
                   │
          ┌────────┴────────┐
          ▼                 ▼
      Text Reply       Voice Reply
```

---

# 📋 What FinMate AI Can Do

- Analyze bank statements
- Answer transaction-related questions
- Track expenses
- Detect recurring subscriptions
- Categorize spending
- Identify income sources
- Calculate monthly expenses
- Find the largest transactions
- Summarize spending patterns
- Suggest saving opportunities
- Support voice conversations

---

# 📂 Workflow 1 — Finance RAG

Automatically:

- Monitors a Google Drive folder
- Downloads newly uploaded files
- Extracts document text
- Splits documents into chunks
- Creates embeddings
- Stores vectors in Pinecone

This workflow keeps the knowledge base updated without manual intervention.

---

# 🤖 Workflow 2 — FinMate AI

Users interact through Telegram using text or voice.

The assistant:

- Understands natural language
- Searches the Pinecone knowledge base
- Retrieves relevant financial information
- Generates accurate responses
- Converts replies into voice when needed

---

# 🚀 Installation

## Clone the Repository

Clone this repository:

```bash
git clone https://github.com/yourusername/finance-rag-pipeline.git
```

Or, if you're using the complete FinMate AI project that contains both workflows:

```bash
git clone https://github.com/yourusername/finmate-ai.git
```

2. Import both workflows into n8n.

3. Configure credentials:
   - Telegram
   - Google Drive
   - Pinecone
   - Hugging Face
   - OpenRouter
   - Groq
   - AssemblyAI

4. Activate the **Finance-RAG** workflow.

5. Upload your financial documents to the configured Google Drive folder.

6. Activate the **AI Personal Finance Manager** workflow.

7. Start chatting with your Telegram bot.

---

# 📌 Future Improvements

- WhatsApp Integration
- OCR for scanned PDFs
- Multi-language support
- Budget Planner
- Investment Insights
- Email Reports
- Web Dashboard
- Expense Charts
- Monthly Financial Reports

---

# 👨‍💻 Author

**Sanskar Parab**

⭐ If you found this project useful, consider giving it a star on GitHub!
