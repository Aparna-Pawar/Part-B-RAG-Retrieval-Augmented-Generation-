# Part B – RAG (Retrieval-Augmented Generation)

This part implements a RAG document Q&A chatbot that answers questions from uploaded documents.  
Upload the document and hold on a few seconds until it is loaded, split, stored in a vector database, and retrieved

## Tools & Libraries You Used

- Python 3 – Core programming language.
- Streamlit – For building and deploying the interactive chatbot apps.
- LangChain – For building the RAG pipeline and handling document retrieval.
- Groq API – Used as the LLM backend (instead of OpenAI).
- dotenv – For loading API keys securely from a .env file.
- FAISS – Vector database for storing and retrieving embeddings.
- PyPDF2/PDF loader – For document loading in RAG mode.

## 📂 Folder Structure
app.py - Main RAG pipeline code.
requirements.txt - Python dependencies.
.env - Stores the secret keys like GROQ_API_KEY, LANGCHAIN_API_KEY (Create your own Groq API key and Langchain API key for running app.py)

## Setup Instructions

1. Clone the repo:
bash
git clone https://github.com/Aparna-Pawar/Part-B-RAG.git
cd Part-B-RAG

2. Create and activate a virtual environment:
- python3 -m venv venv
- source venv/bin/activate   # macOS/Linux
- venv\Scripts\activate      # Windows

3. Install dependencies:
pip install -r requirements.txt

4. If your version requires API keys for any service, create a .env file and add your own API keys:

- YOUR_API_KEY_NAME=your_api_key_here 
  (e.g. GROQ_API_KEY="your_api_key")

Run Streamlit Locally 
streamlit run rag_app.py

- Upload documents (PDF).
- The chatbot retrieves relevant content from the uploaded documents.
- Users can ask questions, and answers are generated from the retrieved content.

⚠️ Limitationsz;
- Requires users to provide their own API keys (Groq API Key).
- Model answers depend on retrieval quality + Groq model output, so incorrect or incomplete answers are possible if documents are not well structured. So please use the documents which are provided in a repo.
- Currently supports only text/PDF documents

☁️ Access Online

You can also access the RAG chatbot directly on Streamlit Cloud:
https://6kujujvabcmsxrozvnrdq6.streamlit.app/
