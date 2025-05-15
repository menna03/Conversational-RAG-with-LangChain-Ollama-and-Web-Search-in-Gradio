# Conversational-RAG-with-LangChain-Ollama-and-Web-Search-in-Gradio


🎯 Goal:
Create a Conversational RAG (Retrieval-Augmented Generation) chatbot using:

Ollama (LLaMA3) for the LLM

Nomic embeddings

FAISS vector store for LangChain docs

SerpAPI for real-time web search

Python REPL tool

Gradio for the chatbot interface

🧠 Key Components:
LLM & Embeddings Initialization:

Loads llama3 model using Ollama.

Loads nomic-embed-text model for embeddings.

Vector Store Setup:

Loads or creates a FAISS vector store from markdown docs in langchain_docs/.

Documents are split into chunks and embedded.

Only 50 chunks are used to keep things light.

Tools Defined:

RAG Tool: Retrieves similar content from LangChain docs.

SerpAPI Search Tool: Answers current or general queries using the web.

Python REPL Tool: Executes Python code queries live.

Agent Setup:

Combines tools and LLM using LangChain's initialize_agent with memory support (chat history).

Enables smart decision-making: chooses whether to search, use docs, or run code.

Gradio UI:

Provides a chat interface for user interaction.

Uses chat_with_agent() to handle messages and generate responses.

✅ What You Can Do with It:
Ask questions about LangChain.

Search the internet in real time.

Run Python code like a calculator.

Interact in a conversational manner with memory.




📚 Main Documentation Portal
🔗 https://docs.langchain.com/

📄 Core Components Docs
Getting Started
🔗 https://docs.langchain.com/docs/get-started/introduction

Quickstart Guide
🔗 https://docs.langchain.com/docs/get-started/quickstart

Components Overview
🔗 https://docs.langchain.com/docs/components/

Retrieval
🔗 https://docs.langchain.com/docs/modules/data_connection/retrieval/

Memory
🔗 https://docs.langchain.com/docs/modules/memory/

Chains
🔗 https://docs.langchain.com/docs/modules/chains/

Agents
🔗 https://docs.langchain.com/docs/modules/agents/

Callbacks
🔗 https://docs.langchain.com/docs/modules/callbacks/

🛠️ Ecosystem Integrations
Tools & Plugins
🔗 https://docs.langchain.com/docs/integrations/tools/

Vector Stores
🔗 https://docs.langchain.com/docs/integrations/vectorstores/

LLM Providers
🔗 https://docs.langchain.com/docs/integrations/llms/

👨‍💻 API Reference (for Developers)
LangChain Python API
🔗 https://api.python.langchain.com/en/latest/

LangChainJS (JavaScript/TypeScript)
🔗 https://js.langchain.com/docs/

