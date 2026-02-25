# rag-chatbot
Simple RAG chatbot demo using LangChain, Google Gemini, and Chroma.

- Notebook: `rag_chatbot.ipynb` (open in Colab or run locally)
- Loads a PDF, splits into chunks, embeds with `gemini-embedding-001`
- Stores embeddings in Chroma (`./chroma_db`) and retrieves top-k chunks
- Answers questions with `gemini-2.5-flash` using retrieved context

Run:
1) Open `rag_chatbot.ipynb` and install the pip dependencies in the first cell  
2) Set `GOOGLE_API_KEY` (and optional LangChain tracing keys)  
3) Update the PDF path in the loader cell, run all cells, then ask questions
