# 🧠 MediChatAI

An end-to-end medical chatbot powered by semantic search and LLMs. Ingests trusted medical knowledge from the *Gale Encyclopedia of Medicine* and delivers intelligent, context-aware answers using OpenAI or local LLaMA models.

---

## 🚀 Features

- 📚 Ingests structured medical content from Gale’s Encyclopedia  
- 🧩 Chunks text and builds vector embeddings  
- 🔎 Semantic search with Pinecone vector DB  
- 💬 User queries are matched and routed to LLMs  
- 🤖 Supports both OpenAI API and local LLaMA models  
- 🛠️ Built with Python, LangChain, Flask, and Pinecone  

---

## 🧰 Tech Stack

- **Python** – Core development  
- **LangChain** – Chain LLMs and vector DB logic  
- **Flask** – Backend API  
- **Pinecone** – Vector database for semantic retrieval  
- **OpenAI / LLaMA** – LLMs for generating responses  

---

## ⚙️ How It Works

1. **Data Ingestion**  
   Medical knowledge is sourced from the *Gale Encyclopedia of Medicine*.

2. **Preprocessing & Chunking**  
   Content is split into manageable text chunks.

3. **Vectorization**  
   Each chunk is converted into an embedding using a selected embedding model.

4. **Semantic Indexing**  
   Embeddings are stored in Pinecone for fast, semantic search.

5. **Query Handling**  
   - User inputs a question via frontend.  
   - Query is embedded and matched against the knowledge base.  
   - Top results are retrieved and passed to an LLM.

6. **Response Generation**  
   - LLM (OpenAI or LLaMA) generates the final answer using retrieved context.

---

## 🔧 Setup Instructions

```bash
# Clone the repo
git clone https://github.com/your-username/MediChatAI.git
cd MediChatAI

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Create a .env file and add your keys:
OPENAI_API_KEY=your_openai_key
PINECONE_API_KEY=your_pinecone_key
PINECONE_ENV=your_pinecone_env
```
---

## 📬 Example Query

> **“What are common symptoms of Type 2 Diabetes?”**

Returns a precise, LLM-generated response based on retrieved medical content.

---

## 🤝 Contributions

Pull requests are welcome! Please open an issue first for major changes.

---

## 📄 License

MIT License

