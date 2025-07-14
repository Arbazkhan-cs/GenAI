# 🔗 LangChain Chains Tutorial

This folder provides practical examples of how to use **Chains** in LangChain to connect multiple components (models, prompts, tools, parsers) into intelligent, multi-step workflows.

Chains are the building blocks of complex applications like agents, pipelines, and conversational bots.

---

## 📂 File Overview

| File Name                 | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| `1_sequential_chain.py`   | Executes a series of tasks one after the other (step-by-step)               |
| `2_parallel_chain.py`     | Executes multiple tasks at the same time and aggregates the results         |
| `3_conditional_chain.py`  | Executes different chains based on conditions or logic (if-else branching)  |

---

## 🤖 What Are Chains?

Chains allow you to:

- Compose multiple LangChain components (e.g. prompt → model → parser)
- Build **modular** and **reusable** pipelines
- Add **logic** between tasks (sequential, parallel, or conditional)

LangChain supports:
- `SimpleChain`, `SequentialChain`, `LLMChain`, `ConditionalChain`, etc.

---

## 🚀 How to Run

Install dependencies:

```bash
pip install -r requirements.txt
````

Run any file directly:

```bash
python 1_sequential_chain.py
```

---

## 🔍 Example: Sequential Chain

```python
from langchain.chains import SequentialChain

# Chain 1: Generate a blog title
# Chain 2: Generate a blog outline based on the title

# Outputs from Chain 1 are passed into Chain 2
```

---

## 🧠 Use Cases

* 🧾 **Document generation:** Title → Outline → Section text
* 🧠 **Question answering:** Query → Context → Answer
* 🛠 **Tool use:** Input → Tool call → Result → Final response
* 🔄 **Decision trees:** Based on logic or model response

---

## 📚 References

* [LangChain Docs – Chains](https://docs.langchain.com/docs/components/chains)
* [LangChain GitHub](https://github.com/hwchase17/langchain)

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.
