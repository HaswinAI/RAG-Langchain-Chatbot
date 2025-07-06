📚 RAG Chatbot using LangChain + Groq
This is an interactive AI chatbot that answers questions from uploaded PDF documents using RAG (Retrieval-Augmented Generation) with LangChain and Groq-hosted LLMs (like LLaMA 3). It's built using Streamlit, FAISS, and HuggingFace embeddings.

🚀 Features
Upload any PDF document 📄

Automatically reads and chunks the content

Embeds using sentence-transformers/all-MiniLM-L6-v2

Stores chunks in a FAISS vector store

Uses Groq's blazing-fast LLMs (like llama3-70b-8192)

Answers questions contextually from the uploaded document

Built with LangChain, Streamlit, and Groq

🧠 Tech Stack
Tool	Purpose
🦜 LangChain	Framework for LLM pipelines
🧠 Groq	LLM inference (LLaMA 3 / Mixtral)
🧠 HuggingFace Embeddings	Embedding PDF chunks
🗃 FAISS	Fast vector similarity search
📑 PyPDF2	Reading PDF text
🎛 Streamlit	Web interface
🔐 Dotenv	API key management

📁 Project Structure
bash
Copy
Edit
RAG_chatbot/
├── app.py                  # Main Streamlit interface
├── utils.py                # PDF loading & chunking
├── rag_chain.py            # Embedding, retrieval, QA chain
├── .env                    # API key config (not pushed to GitHub)
├── requirements.txt        # All required libraries
├── README.md               # Project documentation
└── data/                   # Uploaded PDFs (stored temporarily)
🧪 Demo
<!-- Optional: add screenshot -->

🛠 Installation
1. Clone the repo
bash
Copy
Edit
git clone https://github.com/your-username/rag-chatbot-groq.git
cd rag-chatbot-groq
2. Create a virtual environment
bash
Copy
Edit
python -m venv chatbot
source chatbot/bin/activate  # On Windows: chatbot\Scripts\activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Set your Groq API key
Create a .env file:

ini
Copy
Edit
GROQ_API_KEY=your_actual_groq_key_here
▶️ Run the App
bash
Copy
Edit
streamlit run app.py
Open your browser at http://localhost:8501 and upload a PDF to chat with it!

💡 Example Use Cases
Query research papers for quick insights

Analyze annual reports

Understand company policies

Legal document Q&A

Student note assistant

🔒 Disclaimer
This project is for educational/demo purposes. It does not store user data or document contents permanently.

📄 License
MIT License

✨ Acknowledgements
LangChain

Groq

Streamlit

FAISS

