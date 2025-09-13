# Groq-Powered Conversation Management & JSON Extraction

This project demonstrates an advanced **conversation management system** integrated with the **Groq AI platform** (OpenAI-compatible) to perform automated conversation summarization and structured data extraction from chat messages. It leverages the power of **LLM-based models**, **JSON schema validation**, and **function calling** to build robust and scalable AI-driven tools for chat applications, mobile assistants, and customer support systems.

---

## 🔹 Features

### 1. Conversation Management
- Tracks the conversation history dynamically.
- Automatically summarizes conversations after a configurable number of turns (`summarization_trigger_k`).
- Maintains an **auto-summary** at the start of the conversation for quick context reference.
- Supports:
  - Truncating messages by number of turns
  - Truncating by character limits
  - Truncating by word limits
- Ensures that conversation history stays concise and manageable for AI processing.

### 2. Automated Summarization
- Generates concise summaries capturing **key points, actions, and entities**.
- Works automatically at every Nth message or manually on-demand.
- Uses **Groq-compatible models** (`llama-3.1-8b-instant`) for generating high-quality summaries.
- Fallback logic ensures summarization even if the API call fails.

### 3. JSON Function Calling
- Extracts structured information from chat text such as:
  - Name
  - Email
  - Phone number
  - Location
  - Age
- Enforces **JSON Schema validation** to ensure correctness.
- Provides automatic handling of missing values (`null`) and optional fields.

### 4. Groq API Integration
- Fully compatible with **Groq AI API** endpoints.
- Uses **OpenAI-compatible Python client** for chat completions and function calling.
- Supports advanced features like **forced function calls** to extract structured JSON data from unstructured text.

### 5. Demo Use Cases
- Chatbot development with auto-summary and context preservation.
- Mobile app support (example: fertilizer recommendation app) with periodic summaries.
- Contact information extraction and validation from user conversations.

---
