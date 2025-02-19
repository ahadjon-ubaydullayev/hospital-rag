# Hospital RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot for hospital systems, powered by **LangChain** and **Neo4j**. It answers complex queries using both structured (e.g., patient records, locations) and unstructured (e.g., reviews) data.

## Features
- Natural language querying of hospital data
- Neo4j graph database integration
- Modular LangChain workflows for retrieval and generation
- FastAPI backend and Streamlit frontend
- Dockerized deployment (Neo4j, API, UI)

## Prerequisites
- Python 3.9+
- Docker and Docker Compose
- OpenAI API key
- Neo4j AuraDB instance

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ahadjon-ubaydullayev/hospital-rag-chatbot.git
   cd hospital-rag-chatbot
