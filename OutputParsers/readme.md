# 🧾 LangChain Output Parsers Tutorial

This folder provides practical examples for using **Output Parsers** in the LangChain framework to convert raw LLM responses into structured, validated, and usable formats.

Output Parsers are essential when working with LLMs for real-world tasks where the **structure and reliability of the output matters** (e.g., APIs, databases, forms).

---

## 📂 File Overview

| File Name                    | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `1_StrOutputParser.py`      | Basic parser that returns output as a raw string                            |
| `2_JsonOutputParser.py`     | Parses model output as valid JSON (dictionary or list)                      |
| `3_StructuredOutputParser.py` | Creates structured outputs using manually defined schemas                    |
| `4_PydanticOutputParser.py` | Parses outputs into Python objects using [Pydantic](https://docs.pydantic.dev/) models |

---

## 🎯 Why Use Output Parsers?

LLMs usually return raw strings. But in real-world apps, you often need:

- ✅ Well-formatted JSON for APIs
- ✅ Typed data models for backend logic
- ✅ Reliable structures for databases
- ✅ Easy debugging and validation

LangChain's Output Parsers help bridge that gap.

---

## 🚀 How to Use

Install dependencies:

```bash
pip install -r requirements.txt
````

Run any script directly:

```bash
python 2_JsonOutputParser.py
```

---

## 🧪 Example: JSON Output Parser

```python
from langchain.output_parsers import JsonOutputParser

parser = JsonOutputParser()
response = '{"name": "Arbaz", "role": "AI Engineer"}'
parsed = parser.parse(response)
print(parsed["name"])  # Output: Arbaz
```

---

## 🧱 Pydantic Output Example

```python
from pydantic import BaseModel
from langchain.output_parsers import PydanticOutputParser

class User(BaseModel):
    name: str
    age: int

parser = PydanticOutputParser(pydantic_object=User)
output = parser.parse('{"name": "Arbaz", "age": 26}')
print(output.name)  # Output: Arbaz
```

---

## 🔐 Use Cases

* Extracting structured data from LLM outputs
* Building chatbots that return typed responses
* Backend services needing clean, validated data
* Filling forms or storing output in databases

---

## 🧑‍💻 Author

**Arbaz Khan**
[GitHub](https://github.com/Arbazkhan-cs) • [LinkedIn](https://www.linkedin.com/in/arbazkhan-cs/)

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 📚 References

* [LangChain Output Parsers](https://docs.langchain.com/docs/components/output_parsers)
* [Pydantic Docs](https://docs.pydantic.dev/)
* [LangChain GitHub](https://github.com/hwchase17/langchain)

