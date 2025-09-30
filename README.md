# Part B – RAG (Retrieval-Augmented Generation)

This part implements a RAG document Q&A chatbot that answers questions from uploaded documents.  
Upload the document and wait a few seconds until it is loaded, split, stored in a vector database, and retrieved

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
python3 -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

3. Install dependencies
pip install -r requirements.txt

4. If your version requires API keys for any service, create a .env file and add your own API keys:

YOUR_API_KEY_NAME=your_api_key_here 
(e.g. GROQ_API_KEY="your_api_key")

Run Streamlit Locally 
streamlit run rag_app.py

- Upload documents (PDF).
- The chatbot retrieves relevant content from the uploaded documents.
- Users can ask questions, and answers are generated from the retrieved content.

