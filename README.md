

# 🧠 Interactive Trading Chatbot using LLM (LLaMA 3.1 + Langchain)

An AI-powered **interactive trading chatbot** built using **ChatGroq (LLaMA-3.1-8B)**, **OllamaEmbeddings**, **FAISS**, and **Langchain**. This chatbot provides real-time, accurate answers to trading-related queries by retrieving and understanding contextual information from documents.

---

## 📌 Features

- ✅ Chat with a custom-trained LLM on trading documents
- ⚡ Fast and accurate answers using **vector search (FAISS)**
- 🔗 Powered by **Langchain** for chaining and memory
- 📄 Custom document ingestion & processing
- 🧩 Embeddings via **OllamaEmbeddings**
- 🎯 Purpose-built to **reduce customer care workload**

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/prathmeshpatil98/Trading_chatbot.git
cd Trading_chatbot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Make sure you have Python 3.9+ installed.

### 3. Run Ollama and Load LLaMA Model

Install Ollama and pull the model:

```bash
ollama run llama3
```

> You can use other LLMs compatible with Ollama as well.

### 4. Prepare Documents

Put your trading-related documents in the `/docs` folder.

---

## 🛠️ How It Works

### 🧱 Components

| Component              | Description                                                   |
|------------------------|---------------------------------------------------------------|
| **LLM Backend**         | ChatGroq with LLaMA-3.1-8B                                     |
| **Embeddings**          | OllamaEmbeddings for text vectorization                      |
| **Vector Store**        | FAISS for fast similarity search                             |
| **Chain**               | Langchain ConversationalRetrievalChain                       |
| **Document Processing** | Langchain loaders and text splitters                         |

### 🔄 Workflow

1. **Load and preprocess documents**
2. **Generate embeddings with Ollama**
3. **Store vectors using FAISS**
4. **User inputs question**
5. **System searches similar docs & generates an answer using LLM**

---

## 💬 Example Usage

```python
response = qa_chain.run("What is the best trading strategy in volatile markets?")
print(response)
```

---

## 🧠 Future Improvements

- [ ] Add GUI with Streamlit or Gradio
- [ ] Live chat support integration
- [ ] Fine-tune LLM on domain-specific FAQs
- [ ] Support for real-time document updates

---

## 📞 Support

For any questions or support, open an issue or contact prthmeshpatil98@gmail.com

---

## 🪪 License

This project is licensed under the MIT License.
