# 🤖 Legal Assistant with RAG

A simple legal assistant using **RAG (Retrieval-Augmented Generation)** and **LangChain**, focused on comparing responses from a Gemini Flash 1.5 LLM **with and without retrieval**. This project is built around Iranian civil law.

---

## 🔍 What It Does

* Uses **LangChain's RAG pipeline** to retrieve legal content from indexed Persian law documents.
* Sends queries to **Gemini Flash 1.5** LLM:

  * Once with retrieved context (RAG mode)
  * Once without any context (plain LLM mode)
* Displays and compares both answers for better legal evaluation.

---

## 🧠 Technologies Used

* **LangChain** for retrieval and orchestration
* **Gemini Flash 1.5** as the large language model
* **FAISS / Chroma** for embedding search (pluggable)
* **IPython Widgets** for interactive notebook interface
* **Markdown** for rich display of legal answers

---

## ⚙️ Setup

```bash
# Clone the repo
$ git clone https://github.com/your-username/legal-assistant-rag.git


```

---

## 🧪 Example Usage

1. Load Iranian civil law (e.g. مواد ۳۳۸ تا ۳۸۰)
2. Ask a legal question:

```text
در صورت وجود عیب پنهانی در مبیع، چه حقوقی برای مشتری در نظر گرفته شده است؟
```

3. The assistant compares answers:

* ✅ **With RAG:**

  > مشتری حق فسخ یا مطالبه تفاوت قیمت دارد.
  > 📌 ماده ۳۵۷ و ۳۷۳ قانون مدنی

* ❌ **Without RAG:**

  > بسته به قانون کشور، خریدار ممکن است حق فسخ داشته باشد...

---

## 📁 Project Structure

```
legal-assistant-rag/
├── data/                # Persian legal documents
├── rag/                 # RAG pipeline setup
├── llm/                 # Gemini Flash query logic
├── notebook.ipynb       # Interactive demo notebook
├── utils/               # Text processing utilities
└── README.md
```

---

## ✅ Future Ideas

* Add document metadata (e.g. ماده number, باب)
* Extend to multiple legal codes (تجارت، کیفری)
* Support for contract clause validation
* Streamlit or FastAPI frontend

---



## 📜 License

MIT License – Free to use and extend.
