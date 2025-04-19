# Retrieval-Augmented Generation (RAG) Demo

This repository demonstrates a basic Retrieval-Augmented Generation (RAG) pipeline using [LangChain](https://github.com/langchain-ai/langchain) and OpenAI models. The notebook loads a sample document, splits it into chunks, creates embeddings, builds a FAISS vector store, and enables question answering over the content using a retrieval-augmented LLM.

## Features

- Loads and splits a sample document
- Creates embeddings with OpenAI
- Stores vectors using FAISS
- RetrievalQA and Conversational RetrievalQA chains
- Custom prompt template for grounded answers

## Requirements

- Python 3.8+
- OpenAI API key

## Installation

Install dependencies (run in your notebook or terminal):

```python
!pip install -U langchain-community
!pip install langchain langchain-openai pypdf faiss-cpu tiktoken
```

## Usage

1. **Set your OpenAI API key**  
   Make sure your OpenAI API key is available as an environment variable:
   ```python
   import os
   os.environ["OPENAI_API_KEY"] = "your-openai-api-key"
   ```

2. **Run the notebook**  
   Execute each cell in `rag.ipynb` to:
   - Load and split the sample document
   - Create embeddings and vector store
   - Set up the RAG pipeline
   - Ask questions and get answers

3. **Conversational QA**  
   The notebook also demonstrates a conversational retrieval chain for multi-turn interactions.

## Customization

- Replace `sample_document.txt` with your own documents for custom retrieval.
- Change the model name in `ChatOpenAI` if you have access to other OpenAI models.

## Example Questions

- What is RAG?
- When was RAG introduced?
- What are the key components of a RAG system?

## License

MIT License

---

*This project is for educational purposes and demonstrates basic RAG concepts using LangChain and OpenAI APIs.*
