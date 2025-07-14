# 🧠 Embedding Models Examples

This directory provides simple, standalone Python scripts to help you understand how to use **embedding models**—both **cloud-hosted (via Hugging Face Hub)** and **locally running models**—for applications like search, RAG (Retrieval-Augmented Generation), and semantic similarity.

---

## 📂 File Overview

| File Name                  | Description                                                            |
|---------------------------|------------------------------------------------------------------------|
| `1_embedding_hf.py`       | Shows how to use Hugging Face-hosted embedding models via API          |
| `2_local_embedding_model.py` | Demonstrates how to load and use embedding models locally without internet |

---

## ✅ What Are Embeddings?

Embeddings convert text into numerical vectors that capture semantic meaning. These can be used for:

- Semantic search and ranking  
- Clustering and categorization  
- Similarity comparison  
- Retrieval in RAG pipelines

---

## 🚀 Usage

### 1️⃣ Hugging Face Hosted Embeddings (`1_embedding_hf.py`)

```bash
python 1_embedding_hf.py
````

✅ Make sure you have a Hugging Face access token:

```env
HUGGINGFACEHUB_API_TOKEN=your_token_here
```

This uses models like:

* `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2`
* `intfloat/multilingual-e5-large`

---

### 2️⃣ Local Embedding Model (`2_local_embedding_model.py`)

```bash
python 2_local_embedding_model.py
```

✅ Make sure you've downloaded the model first, or allow auto-download on first run.

Works offline and is ideal for:

* Privacy-sensitive tasks
* No-internet environments
* Edge devices and Raspberry Pi setups (lightweight models)

---

## 📦 Requirements

* Python 3.8+
* Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🔍 Example Output

```text
Original Text: भारत का प्रधानमंत्री कौन है?
Vector Length: 768
Sample Values: [0.012, -0.090, 0.056, ...]
```

---

## 🧠 Recommended Models

| Model Name                              | Description                          | Vector Dim |
| --------------------------------------- | ------------------------------------ | ---------- |
| `paraphrase-multilingual-MiniLM-L12-v2` | Lightweight, multilingual            | 768        |
| `intfloat/multilingual-e5-large`        | High-performance for retrieval tasks | 1024       |

---

## 📚 References

* [LangChain Embeddings Docs](https://docs.langchain.com/docs/components/embeddings)
* [Hugging Face Sentence Transformers](https://huggingface.co/sentence-transformers)

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan/)

---

## 📄 License

This project is licensed under the **MIT License**.
