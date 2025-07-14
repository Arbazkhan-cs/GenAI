# 📝 LangChain Prompts & Messages Tutorial

This folder contains practical, hands-on examples for working with **prompts** and **messages** in the LangChain framework. It walks through how to create, format, store, and use prompts effectively—including chat-specific prompts and message orchestration.

---

## 🧠 What Are Prompts?

In LangChain, prompts are formatted instructions sent to LLMs. Crafting prompts well is crucial for getting accurate and relevant outputs from language models.

LangChain supports:
- `PromptTemplate`: For simple text generation
- `ChatPromptTemplate`: For structured conversational input (role-based)
- `System`, `Human`, and `AI` Messages: To simulate multi-turn interactions

---

## 📂 File Overview

| File Name                        | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| `1_promptTemplate.py`           | Basic usage of `PromptTemplate` for static and dynamic prompt construction |
| `2_chatPromptTemplate.py`       | How to use `ChatPromptTemplate` for role-based messages                    |
| `3_messages.py`                 | Demonstrates LangChain's `SystemMessage`, `HumanMessage`, and `AIMessage`  |
| `4_promptTemplate_application.py` | Applying prompt templates in a real application-like scenario              |
| `5_save_template.py`            | How to save/load prompt templates using JSON (`research_paper_prompt_template.json`) |
| `6_Conversational_Chatbot.py`   | A functional conversational chatbot using chat prompts and LangChain messages |

---

## 📘 JSON File

- **`research_paper_prompt_template.json`**  
  Stores a structured prompt template to guide the generation of academic-style content.

---

## 🚀 Usage

Install dependencies:

```bash
pip install -r requirements.txt
````

Run any script:

```bash
python 1_promptTemplate.py
```

---

## 🧪 Key Features

✅ Dynamically substitute variables in prompts
✅ Role-based prompt modeling for chat use cases
✅ Save and reuse templates
✅ Simulate conversational memory using messages
✅ Build production-ready prompts for academic, chatbot, or search use cases

---

## 🔍 Example: Chat Prompt Template

```python
from langchain.prompts.chat import ChatPromptTemplate
from langchain.schema import HumanMessage, SystemMessage

prompt = ChatPromptTemplate.from_messages([
    ("system", "You are a helpful assistant."),
    ("human", "{user_input}")
])
final_prompt = prompt.format_messages(user_input="Explain LLMs in simple terms.")
```

---

## 💡 Real-World Applications

* Chatbots with memory and role-awareness
* Template-based document generation
* Controlled query generation for search engines
* Academic paper or resume generation tools

---

## 🧠 Best Practices

* Keep prompts concise but informative
* Use system messages to guide tone and behavior
* Leverage `ChatPromptTemplate` for complex role-based use cases
* Save reusable templates in `.json` for team collaboration

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.
