# 🤖 AI Store Support Chatbot — n8n + RAG

Automated customer support agent built with n8n, Qdrant, and LLaMA 3.3-70b.

## 🚀 Features

| Feature | Description |
|---|---|
| 🔍 RAG Pipeline | Retrieves answers from Qdrant vector store |
| 🧠 LLaMA 3.3-70b | Fast responses via Groq Cloud |
| 🌐 Multilingual | Replies in customer's language automatically |
| 💬 Memory | Retains last 10 messages for context |
| 📦 Vector Store | Google Gemini embeddings stored in Qdrant |

## 🛠️ Stack

| Layer | Tool |
|---|---|
| Orchestration | n8n |
| LLM | Groq — LLaMA 3.3-70b-versatile |
| Embeddings | Google Gemini (PaLM API) |
| Vector DB | Qdrant |
| Memory | n8n Buffer Window (10 messages) |

## 📂 Workflow Structure

| Node | Role |
|---|---|
| Manual Trigger + Edit Fields | Loads store policy text |
| Qdrant Vector Store (insert) | Embeds and stores policy data |
| Chat Trigger | Receives customer messages |
| AI Agent | Orchestrates responses with RAG |
| Groq Chat Model | Generates natural language replies |
| Simple Memory | Maintains conversation history |
| Qdrant Vector Store (tool) | Retrieves relevant store info |

## 📋 Store Knowledge Base

- Delivery within Baku: 1–2 business days
- Delivery to regions: 3–5 business days
- Free delivery on orders over $50
- Return period: 14 days (receipt + original packaging required)
- Payment: cash, card, bank transfer
