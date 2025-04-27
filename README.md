# RAG_FLASK_LANGCHAIN_FAISS_LANGSMITH
Mahabharatha & Ramayana Q&A System

📚 Mahabharatha & Ramayana Q&A System (Flask + LangChain + FAISS)
This project builds an intelligent Question Answering (QA) system based on the ancient Indian epics Mahabharatha and Ramayana, using LLMs, FAISS, LangChain, and Flask.

Ask any natural language question about these epics, and get contextual, accurate answers — powered by AI!

✨ Features
📖 Extracts text from uploaded PDFs (Mahabharatha, Ramayana)

🧩 Splits and stores text chunks into a FAISS vector database for fast retrieval

🧠 Uses HuggingFace Embeddings to embed texts

🔥 Uses Groq's LLaMA 3 8B model (via ChatGroq) for answering

🛡️ Provides source attribution (shows filename and page number)

🌈 Stylish, responsive Flask web UI

🔍 LangSmith observability integrated

🏗️ Tech Stack
Python 3.11+

Flask (Web Application)

LangChain (Orchestration)

Groq LLaMA 3 8B (Language Model)

HuggingFace Sentence Transformers (Embeddings)

FAISS (Vector Search Engine)

PyPDF2 (PDF Text Extraction)

LangSmith (Tracing and Observability)

🚀 Setup Instructions
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/yourusername/mahabharatha-ramayana-qa.git
cd mahabharatha-ramayana-qa

2. Install Dependencies

pip install -r requirements.txt

If you have issues with FAISS on Windows, run:
pip install faiss-cpu --index-url https://pypi.fury.io/conda-forge/

3. Prepare Your Data
Create a folder named pdfs/ in the project root.

Add Mahabharatha.pdf and Ramayana.pdf inside it.
/pdfs
  ├── mahabharatha.pdf
  └── ramayana.pdf
  
4. Setup .env
Create a .env file in the project directory and add:
LANGCHAIN_TRACING_V2=true
LANGCHAIN_API_KEY=your_langsmith_api_key
LANGCHAIN_ENDPOINT=https://api.smith.langchain.com
GROQ_API_KEY=your_groq_api_key
(You can skip LANGCHAIN_API_KEY if you don't want tracing.)

🏃 Run the Application
python app.py
Open http://127.0.0.1:5000/ in your browser and start asking questions!

🖼️ UI Preview
🎨 Centered Input Field
📚 Colorful Background
📝 Clean Display of Answers and Source References


