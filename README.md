# n8n-whatsapp-ai-voice-bot
Advanced WhatsApp AI Chatbot built on n8n. Supports voice messages (STT/TTS), Supabase context retrieval, file handling, and JavaScript data cleaning.
# 🤖 Advanced WhatsApp AI Voice & Chat Bot (n8n + Supabase)

A production-ready, highly advanced AI Chatbot workflow built using **n8n**. This system transforms a standard WhatsApp number into an intelligent virtual assistant capable of understanding and responding to both text and **voice messages**, backed by a custom corporate knowledge base.

## 🚀 Key Features

- **Multimodal AI (Text & Voice):** Integrates Speech-to-Text (STT) to understand customer voice notes and Text-to-Speech (TTS) to reply with natural-sounding audio messages.
- **Dynamic RAG System:** Connects directly with **Supabase** to retrieve real-time company information, pricing, and documents to ensure accurate, non-hallucinated answers.
- **Smart Data Cleaning (JavaScript):** Features custom JavaScript nodes to parse AI outputs, sanitizing voice-bound data by automatically stripping out links, raw markdown, and emojis for a flawless text-to-speech rendering.
- **Media & File Handling:** Capable of sending PDF catalogs, invoices, and images dynamically based on user requests.

## 🛠️ Built With

- **n8n** (Workflow Orchestration & Node Logic)
- **Supabase** (Vector Database & Corporate Knowledge Base)
- **OpenAI / Qwen / Groq API** (For advanced LLM reasoning & STT/TTS)
- **WhatsApp Cloud API / Green-API** (Messaging Gateway)
- **Custom JavaScript** (Data parsing and string sanitation)

## 📦 How to Deploy This Workflow

1. **Export/Import:** Download the `workflow.json` file from this repository and import it into your n8n instance.
2. **Database Setup:** Ensure your Supabase instance has a table for your company FAQs or vector embeddings.
3. **Environment Variables:** Configure your API credentials for your WhatsApp provider, AI model, and Supabase inside the respective n8n credentials sections.
4. **Activate:** Set the Webhook node to active and link it to your WhatsApp gateway configuration.

---
*Developed by Ahmed Tamer - AI Automation Engineer*
