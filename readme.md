
# 🚀 LangChain Learning Guide

Welcome to the **LangChain Learning Guide** – a comprehensive, beginner-friendly resource to help you master LangChain, one of the most powerful frameworks for building applications with LLMs (Large Language Models).

![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/Python-3.8+-blue)
![LangChain](https://img.shields.io/badge/LangChain-Guide-orange)

---

## 📚 Table of Contents

- [🔍 Introduction](#-introduction)
- [⚙️ Environment Setup](#️-environment-setup)
- [🧪 Tutorials](#-tutorials)
- [📎 Resources](#-resources)
- [🙌 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🔍 Introduction

[LangChain](https://www.langchain.com/) is a powerful framework for developing applications powered by language models. It enables developers to connect LLMs with external data, tools, and APIs, allowing you to build things like:

- Chatbots
- RAG (Retrieval-Augmented Generation) systems
- Document QA systems
- Autonomous agents
- Text summarizers, and more

This repository is structured to help you understand and experiment with LangChain core concepts through hands-on tutorials.

---

## ⚙️ Environment Setup

To get started:

### 1. Clone the Repository
```bash
git clone https://github.com/Arbazkhan-cs/GenAI.git
cd GenAI
```

### 2. Install Dependencies
Make sure Python 3.8 or higher is installed.

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory and add your credentials:
```env
OPENAI_API_KEY=your_api_key_here
GROQ_API_KEY=your_api_key_here
HUGGINGFACE_API_ACCESS_KEY=your_api_key_here # optional
```

> You may also configure model paths if running local models:
```bash
export LANGCHAIN_MODEL=<path/to/your/model>
```

---

## 🧪 Tutorials

This guide includes modular tutorials categorized by LangChain components:

| Directory            | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| **Agents**           | Learn to build autonomous agents that make decisions using tools and memory.|
| **ChatModels**       | Work with chat-optimized language models (like OpenAI's ChatGPT).           |
| **Chains**           | Compose sequences of calls (chains) to models and tools.                    |
| **EmbeddingModels**  | Generate and use embeddings for vector search and retrieval.                |
| **OutputParsers**    | Parse and format outputs into structured formats (e.g., JSON).              |
| **Prompts**          | Craft and manage prompt templates for dynamic use cases.                    |
| **RAG**              | Build Retrieval-Augmented Generation pipelines with vector stores.          |
| **Runnables**        | Combine components like chains and models into composable functions.        |
| **StructuredOutput** | Enforce structured output from LLMs using schemas and validations.          |
## 📎 Resources

- 📘 [LangChain Documentation](https://docs.langchain.com/)
- 💬 [LangChain Discord Community](https://discord.gg/langchain)
- 🐛 [GitHub Issues](https://github.com/hwchase17/langchain/issues)

---

## 🙌 Contributing

Found a typo? Have suggestions for a new tutorial?

We welcome contributions! Feel free to open a pull request or raise an issue.

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

### ⭐ If you find this project helpful, consider giving it a star on [GitHub](https://github.com/Arbazkhan-cs/GenAI)!

Happy building! 🚀
