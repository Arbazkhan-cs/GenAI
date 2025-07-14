# 🤖 LangChain Chat Models Integration

This repository showcases how to integrate a variety of **chat models**—both **closed-source (e.g., OpenAI, Claude, Gemini)** and **open-source (e.g., Hugging Face Transformers)**—into applications using Python.

Each file provides a self-contained example of how to interact with a specific provider or model using their respective APIs or SDKs.

---

## 📂 File Overview

| File Name                  | Description                                         |
|---------------------------|-----------------------------------------------------|
| `1_google_api.py`         | Use Google Gemini (Generative AI) via Vertex AI API |
| `2_groq_api.py`           | Use Groq's LPU-accelerated API with models like LLaMA |
| `3_openai_api.py`         | Chat with OpenAI models (e.g., GPT-3.5, GPT-4)       |
| `4_anthropic_claude_api.py` | Use Anthropic Claude 3 models via API               |
| `5_huggingface_api.py`    | Use hosted Hugging Face models via Inference API     |
| `6_hf_local.py`           | Run Hugging Face models locally (no internet needed) |

---

## 🎯 Goals

- Demonstrate how to send and receive messages with different chat providers.
- Provide working code snippets for real-world use cases.
- Make it easy to switch between providers for experimentation or benchmarking.
- Support both **cloud-hosted** and **offline** (local) models.

---

## 🛠️ Requirements

- Python 3.8+
- Install dependencies:
```bash
pip install -r requirements.txt
````

* Add your API keys or model configs in a `.env` file:

```env
OPENAI_API_KEY=your_openai_key
ANTHROPIC_API_KEY=your_claude_key
GOOGLE_API_KEY=your_vertex_ai_key
HUGGINGFACEHUB_API_TOKEN=your_hf_token
```

---

## 🚀 How to Use

Run any file directly:

```bash
python 3_openai_api.py
```

Each script contains its own instructions and example prompt/response flow.

---

## 📌 Notes

* For Hugging Face local models, make sure the required model is downloaded.
* Claude and Gemini APIs may require special account access or billing.
* All scripts are minimal and can be extended for use with LangChain, Streamlit, or FastAPI.

---

## 📚 References

* [OpenAI API](https://platform.openai.com/)
* [Anthropic Claude](https://www.anthropic.com/)
* [Google Vertex AI](https://cloud.google.com/vertex-ai)
* [Groq](https://groq.com/)
* [Hugging Face](https://huggingface.co/docs)

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.

```
