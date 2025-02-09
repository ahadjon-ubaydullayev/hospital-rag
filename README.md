```markdown
# Hospital RAG Chatbot

A Retrieval-Augmented Generation (RAG) chatbot for hospital systems, powered by **LangChain** and **Neo4j**. Answers complex queries using structured (patient records, locations) and unstructured (reviews) data.

## Features
- Natural language querying of hospital data
- Neo4j graph database integration
- Modular LangChain workflows for retrieval & generation
- FastAPI backend + Streamlit frontend
- Dockerized deployment (Neo4j, API, UI)

## Prerequisites
- Python 3.9+
- Docker & Docker Compose
- OpenAI API key
- Neo4j AuraDB instance

## Installation
1. Clone repo:
   ```bash
   git clone https://github.com/ahadjon-ubaydullayev/hospital-rag-chatbot.git
   cd hospital-rag-chatbot
   ```
2. Create `.env` file:
   ```env
   OPENAI_API_KEY=your_key
   NEO4J_URI=your_neo4j_uri
   NEO4J_USERNAME=your_username
   NEO4J_PASSWORD=your_password
   ```
3. Start services:
   ```bash
   docker-compose up --build
   ```

## Usage
1. Access Streamlit UI at `http://localhost:8501`
2. Ask questions like:  
   *"Which Austin physicians accept Medicaid managed care?"*

## Project Structure
```
├── api/           # FastAPI backend
├── frontend/      # Streamlit app
├── data/          # Sample data & ETL scripts
├── docker/        # Docker configurations
└── .env.example   # Environment template
```

## Contributing
Follow the [Real Python tutorial](https://realpython.com/build-llm-rag-chatbot-with-langchain/) for base implementation.
