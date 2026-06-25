# 🌐 Real-Time AI Assistant using Ollama, LangChain & DuckDuckGo

## 📌 Overview

Real-Time AI Assistant is an intelligent conversational application that combines Large Language Models (LLMs) with real-time web search capabilities. The system utilizes LangChain, Ollama, DuckDuckGo Search, and Streamlit to provide users with up-to-date information retrieved directly from the internet.

Unlike traditional LLM applications that rely solely on pre-trained knowledge, this assistant retrieves live search results and uses them as context before generating responses, reducing hallucinations and improving answer relevance.

The project demonstrates the practical implementation of Retrieval-Augmented Generation (RAG) principles using real-time web search rather than static document retrieval.

---

## 🎯 Problem Statement

Large Language Models often struggle to provide accurate answers about recent events because their knowledge is limited to training data.

This project addresses that limitation by integrating live web search with an LLM, enabling the assistant to retrieve current information before generating responses.

---

## ✨ Features

### 🌍 Real-Time Web Search

* Retrieves current information from the internet.
* Uses DuckDuckGo Search API for live search results.
* Enables answering questions about recent events and topics.

### 🤖 LLM-Powered Responses

* Uses Llama 3 (8B) running locally through Ollama.
* Generates human-like responses based on retrieved information.

### 🔍 Retrieval-Augmented Generation (RAG)

* Fetches relevant information from web search.
* Injects retrieved context into the LLM prompt.
* Improves factual accuracy and response quality.

### ⚡ Local AI Inference

* Runs entirely on local hardware using Ollama.
* No dependency on paid API services.

### 💬 Conversational Interface

* Interactive chat interface built with Streamlit.
* Maintains conversation history during the session.

### 🛡️ Hallucination Reduction

* Restricts responses to retrieved search results.
* Instructs the model to avoid answering when information is unavailable.

---

## 🏗️ System Architecture

```text
User Question
      │
      ▼
DuckDuckGo Search
      │
      ▼
Search Results
      │
      ▼
Prompt Template
      │
      ▼
Llama 3 (Ollama)
      │
      ▼
Generated Response
      │
      ▼
Streamlit Interface
```

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Frameworks & Libraries

* LangChain
* Streamlit

### LLM

* Llama 3 8B
* Ollama

### Retrieval Tool

* DuckDuckGo Search

### AI Concepts

* Retrieval-Augmented Generation (RAG)
* Prompt Engineering
* Context Injection
* Conversational AI

---

## ⚙️ Workflow

### Step 1: User Query

The user enters a question through the Streamlit chat interface.

### Step 2: Information Retrieval

DuckDuckGo Search retrieves relevant web results based on the user's query.

### Step 3: Context Preparation

Search results are injected into a structured prompt template.

### Step 4: LLM Processing

The prompt is sent to the locally running Llama 3 model through Ollama.

### Step 5: Response Generation

The model generates an answer using only the retrieved context.

### Step 6: Display Output

The response is displayed to the user through the Streamlit interface.

---

## 🧠 AI Concepts Implemented

### Retrieval-Augmented Generation (RAG)

Rather than relying solely on model knowledge, external information is retrieved and supplied as context before response generation.

### Prompt Engineering

A structured prompt instructs the model to:

* Use only retrieved information
* Avoid hallucinations
* Admit when information is unavailable

### Context Grounding

The model's responses are grounded in real-time search results, improving reliability and factual accuracy.

### Local LLM Deployment

The application runs Llama 3 locally using Ollama, eliminating dependence on cloud APIs.

---

## 📊 Sample Interaction

### User

```text
Who won the latest IPL season?
```

### System

```text
Searches DuckDuckGo for current IPL information.
```

### Assistant

```text
Based on the retrieved search results, the winning team was ...
```

---

## 💼 Applications

* AI Research Assistants
* News Summarization
* Current Affairs Chatbots
* Knowledge Retrieval Systems
* Educational Assistants
* Enterprise Information Search

---

## 🚀 Future Enhancements

* Multi-source web search
* Citation and source display
* Search result ranking
* Memory persistence across sessions
* Voice-enabled interactions
* Hybrid search with vector databases
* Agentic tool calling
* Cloud deployment

---

## 👨‍💻 Author

**Chinmaya A S**

Aspiring AI/ML Engineer | Generative AI Developer | LangChain Enthusiast

GitHub: https://github.com/chinmaya-sajeevan

LinkedIn: https://www.linkedin.com/in/chinmaya-a-s
