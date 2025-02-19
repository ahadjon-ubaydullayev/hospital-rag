# Hospital RAG Chatbot

A **Retrieval-Augmented Generation (RAG)** chatbot designed for hospital systems. Powered by **LangChain**, **ChromaDB**, and **OpenAI**, it answers complex queries using both structured (e.g., patient records, locations) and unstructured (e.g., reviews) data.

---

## 🚀 Features

✅ **Natural Language Querying** – Ask questions in plain English and receive precise answers.  
✅ **ChromaDB Vector Store** – Efficient document retrieval with semantic search.  
✅ **Modular LangChain Workflows** – Seamlessly integrates retrieval and generation components.  
✅ **FastAPI Backend & Streamlit Frontend** – Robust API services with an interactive UI.  
✅ **Dockerized Deployment** – Easily deploy the entire system with Docker Compose.  

---

## 📌 Prerequisites

Ensure you have the following installed:

- **Python 3.9+**
- **Docker & Docker Compose**
- **OpenAI API Key**
- **ChromaDB (embedded or hosted)**

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/ahadjon-ubaydullayev/hospital-rag-chatbot.git
cd hospital-rag-chatbot
```

### 2️⃣ Create a `.env` File
Create a `.env` file in the project root with your credentials:

```env
OPENAI_API_KEY=your_openai_api_key
CHROMADB_PATH=chroma_data/
```

### 3️⃣ Install Python Dependencies
Install the required Python packages:

```bash
pip install -r requirements.txt
```

Alternatively, install manually:

```bash
pip install python-dotenv langchain chromadb openai fastapi uvicorn streamlit
```

### 4️⃣ Start the Backend (FastAPI)
Run the FastAPI backend:

```bash
uvicorn api.main:app --reload
```

### 5️⃣ Start the Frontend (Streamlit)
Launch the Streamlit UI:

```bash
streamlit run frontend/app.py
```

### 6️⃣ Run Everything via Docker (Optional)
To run all services using Docker Compose:

```bash
docker-compose up --build
```

---

## 🎯 Usage

### Access the UI:
Visit: [http://localhost:8501](http://localhost:8501)

### Example Queries:
- *"Which Austin physicians accept Medicaid managed care?"*
- *"What are the emergency room wait times?"*

---

---

## 🛠 Contributing

Follow the [Real Python tutorial](https://realpython.com/build-llm-rag-chatbot-with-langchain/) as a base guide.

---

