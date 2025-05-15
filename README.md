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

