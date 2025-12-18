# AI Embeddings, Vector Search & RAG with Gemini

This project demonstrates **end-to-end semantic search and Retrieval-Augmented Generation (RAG)** using **Google Gemini embeddings**, **Sentence Transformers**, **ChromaDB**, and **Gemini LLMs**.

It covers:

* Text embeddings & cosine similarity
* Sentence Transformer embeddings
* Vector database storage & querying (ChromaDB)
* Document chunking & PDF ingestion
* LLM-powered question answering over retrieved context

---

## 📌 Features

* Generate embeddings using **Gemini Embedding API**
* Compute **cosine similarity** between sentences
* Use **SentenceTransformers** for fast local embeddings
* Store and query embeddings in **ChromaDB**
* Build a **basic RAG chatbot** using Gemini LLM
* PDF document ingestion and chunk-based retrieval

---

## 🛠 Tech Stack

* Python
* Google Gemini API (`google-genai`)
* NumPy
* Sentence Transformers
* ChromaDB
* PyPDF
* dotenv

---

## 🔑 Environment Setup

Create a `.env` file in the root directory:

```env
GEMINI_API_KEY=your_api_key_here
```

Install dependencies:

```bash
pip install google-genai sentence-transformers chromadb python-dotenv numpy pypdf
```

---

## 🚀 Project Flow

### 1️⃣ Gemini Embeddings & Cosine Similarity

* Generates embeddings using `gemini-embedding-001`
* Computes cosine similarity between sentences
* Demonstrates semantic similarity vs unrelated queries

---

### 2️⃣ Sentence Transformer Embeddings

* Uses `all-MiniLM-L6-v2`
* Encodes multiple sentences
* Performs similarity search with user queries

---

### 3️⃣ Vector Storage with ChromaDB

* Stores sentence embeddings
* Queries top relevant documents
* Returns distance-based similarity scores

---

### 4️⃣ Document Ingestion (PDF)

* Extracts text from PDF using `PyPDF`
* Splits text into overlapping chunks
* Embeds chunks and stores them in ChromaDB

---

### 5️⃣ RAG Chatbot (LLM + Retrieval)

* Takes user query
* Retrieves top relevant document chunks
* Passes context to Gemini LLM
* Generates grounded answers from retrieved data

---

## 💡 Example RAG Prompt

```text
You are a helpful assistant.
Answer the following query based only on the provided context.

Query: <user_query>

Context:
<retrieved_chunks>
```

---

## 🧠 Key Concepts Demonstrated

* Semantic similarity search
* Vector embeddings
* Retrieval-Augmented Generation (RAG)
* Context grounding for LLMs
* Document-based QA systems

---

## 📈 Use Cases

* AI-powered document chatbots
* Knowledge base search
* Resume / portfolio projects
* Learning vector databases & RAG pipelines

---

## 🏁 How to Run

```bash
python main.py
```

Type your queries and get answers grounded in your documents.

Type `exit` or `quit` to stop the chatbot.

---

## 🔮 Future Improvements

* Add metadata filtering
* Persistent ChromaDB storage
* Multi-document support
* Streaming responses
* Evaluation & feedback loop

---

## 📜 License

This project is for educational and learning purposes.

---

⭐ If you find this useful, feel free to extend it into a production-ready RAG system!
