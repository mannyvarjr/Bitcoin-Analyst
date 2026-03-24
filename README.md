# ₿ Simple Bitcoin AI Analyst (n8n + LangChain)

###  Project Overview
This project is an intelligent **AI Agent** built during my n8n learning journey. Unlike a standard chatbot, this workflow utilizes **Agentic Logic** to decide which tools to use based on a user's question. It can provide historical context from a specific research paper or fetch live market data to give a comprehensive answer about Bitcoin.

###  How It Works
* **Conversational Interface**: Triggered via a chat window where the user asks a question (e.g., "What is the current price?" or "How does mining work?").
* **The "Brain" (AI Agent)**: Uses a **LangChain Agent** powered by **GPT-4o-mini**. The agent analyzes the user's intent to choose the correct path.
* **Tool 1: Live Market Data**: If the user asks for the price, the agent triggers an **HTTP Request** to the CoinGecko API to pull the latest BTC/USD exchange rate.
* **Tool 2: Document Knowledge**: If the user asks about Bitcoin theory, the system downloads a research PDF ("How Bitcoin Works") from **Google Drive**, extracts the text, and provides an answer based on that specific source.
* **Output**: The agent synthesizes the gathered information into a short, professional response.

###  Key Technical Features
* **Agentic Tool-Use**: Demonstrated ability to configure an AI to interact with external APIs and file systems autonomously.
* **RAG (Retrieval-Augmented Generation)**: Implementation of document-based reasoning by extracting text from PDFs to ground the AI's answers in facts.
* **API Integration**: Real-time data fetching using REST APIs.
* **Dynamic Decision Making**: The workflow doesn't just follow a straight line; it branches based on the AI's understanding of the prompt.

###  Tech Stack
* **Automation Platform**: n8n
* **AI Framework**: LangChain (Agent & Chat Model)
* **LLM**: OpenAI GPT-4o-mini
* **External Services**: Google Drive API, CoinGecko API
* **Core Skills**: AI Orchestration, API Management, Document Parsing.
