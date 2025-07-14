# 🔍📚 Retrieval-Augmented Generation (RAG) with LangChain

This repository demonstrates the power of **Retrieval-Augmented Generation (RAG)** using LangChain. It walks through the full RAG pipeline including document loading, splitting, embedding, storing in vector databases, retrieving context, and generating answers via LLMs.

The project includes reusable building blocks and a complete example application: **`youtube_rag.ipynb`**, which extracts transcripts from YouTube videos and enables question answering on them.

---

## 📘 What is RAG?

**Retrieval-Augmented Generation (RAG)** is an advanced NLP technique that **combines traditional retrieval (search)** with **language model generation**.

### ✨ Benefits of RAG

- ✅ Overcomes LLM context length limitations  
- ✅ Provides **factual grounding** from external data  
- ✅ Enables **domain-specific Q&A** and summarization  
- ✅ Reduces hallucination by injecting real content

### 🧠 How It Works

```

```
          [ User Question ]
                 ↓
      ┌─────────────────────┐
      │   Retriever Module  │ ← Vector Store
      └─────────────────────┘
                 ↓
     [ Relevant Context / Chunks ]
                 ↓
      ┌─────────────────────┐
      │    LLM Generation   │ ← Prompt + Context
      └─────────────────────┘
                 ↓
       [ Final Generated Answer ]
```

````

---

## 🧩 Folder Structure

Each subfolder implements a modular component of the RAG pipeline.

| Folder             | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| 📄 `DocumentLoader` | Load raw data from PDFs, web pages, YouTube transcripts, and text files     |
| ✂️ `TextSplitter`   | Split long documents into manageable, context-aware chunks                  |
| 🧠 `VectorStore`    | Store and search vector embeddings using tools like FAISS or Chroma         |
| 🔎 `Retrievers`     | Retrieve relevant chunks based on a user query using similarity search      |

These components can be reused across applications like chatbots, research assistants, or summarizers.

---

## 📒 Main Application: `youtube_rag.ipynb`

This notebook ties everything together in a working pipeline:

1. ✅ Extracts transcript from a YouTube video  
2. ✅ Splits transcript into semantically meaningful chunks  
3. ✅ Embeds chunks and stores them in a vector DB  
4. ✅ Accepts user questions and retrieves relevant content  
5. ✅ Uses an LLM (e.g., OpenAI, Claude, Groq) to generate context-aware answers

```bash
Input: "What is this video about?"
Output: "The video explains how Transformers work using a visual analogy..."
````

---

## ⚙️ Setup Instructions

```bash
pip install -r requirements.txt
```

Add your environment variables in `.env`:

```env
OPENAI_API_KEY=your_key_here
HUGGINGFACEHUB_API_TOKEN=your_hf_token
```

---

## 🚀 To Run the YouTube RAG App

```bash
jupyter notebook youtube_rag.ipynb
```

Make sure you provide a valid YouTube URL with subtitles enabled.

---

## 📚 Resources & Further Reading

* [LangChain RAG Guide](https://docs.langchain.com/docs/use_cases/question_answering/)
* [FAISS for Vector Search](https://github.com/facebookresearch/faiss)
* [ChromaDB](https://www.trychroma.com/)
* [RAG Paper (Facebook AI)](https://arxiv.org/abs/2005.11401)

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.
