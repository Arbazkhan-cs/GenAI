# 🔁 LangChain Runnables Tutorial

This folder contains examples showcasing the **Runnable** interface in LangChain, which is used to compose modular and chainable AI workflows. These Runnables are **building blocks** of modern LangChain pipelines that help in creating **flexible**, **reusable**, and **composable** logic.

---

## 📂 File Overview

| File Name                   | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `1_runnable_sequence.py`    | Executes a linear pipeline (step-by-step flow using `RunnableSequence`)     |
| `2_runnable_parallel.py`    | Runs multiple tasks in parallel and aggregates the results                   |
| `3_runnable_passthrough.py` | Demonstrates a no-op identity operation, useful in dynamic routing           |
| `4_runnable_branch.py`      | Executes different Runnables based on conditional logic (`RunnableBranch`)   |
| `5_runnable_lambda.py`      | Applies a custom function inline using `RunnableLambda`                      |

---

## 🧩 What Are Runnables?

Runnables are **composable units of computation** in LangChain's expression language. They are at the core of:

- LangChain Expression Language (LCEL)
- Chains, Agents, and Tools
- Multi-step LLM workflows

Types of Runnables include:
- `RunnableSequence` – sequential tasks
- `RunnableParallel` – parallel execution
- `RunnableLambda` – custom Python logic
- `RunnableBranch` – if-else branching
- `RunnablePassthrough` – identity function for flow control

---

## 🚀 How to Run

Install dependencies:

```bash
pip install -r requirements.txt
````

Run any script:

```bash
python 1_runnable_sequence.py
```

---

## 🧠 Use Cases

* Chaining prompts, models, and parsers step-by-step
* Running parallel model queries or API calls
* Routing logic through branches based on conditions
* Wrapping custom functions inside pipelines
* Debugging or skipping steps using passthroughs

---

## 🔍 Sample: Runnable Sequence

```python
from langchain_core.runnables import RunnableSequence

# Define a sequence: input -> prompt -> model -> output
chain = RunnableSequence(first_step, second_step, third_step)
result = chain.invoke("input text")
```

---

## 🧠 Best Practices

* Use `RunnableLambda` for quick Python logic without subclassing
* `RunnableBranch` helps in dynamic workflows (like agents)
* Combine `RunnableParallel` with embedding/model calls for speed
* Use `RunnablePassthrough` when you need to conditionally skip a step

---

## 📚 References

* [LangChain Runnables Docs](https://docs.langchain.com/docs/expression_language/runnables)
* [LangChain Cookbook](https://github.com/langchain-ai/langchain-cookbook)
* [LangChain GitHub](https://github.com/langchain-ai/langchain)

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.

