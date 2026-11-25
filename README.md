\# RAG Implementations: Basic \& Advanced



Two implementations of a Retrieval-Augmented Generation (RAG) system developed as part of the \*\*Séminaire et Workshop\*\* university module.



This project explores the evolution of document-based question answering, starting with a simple dense retrieval pipeline and progressing toward an advanced hybrid retrieval architecture.



\## Project Structure



```text

Rag-Implementations/

├── Basic-Rag/

│   └── Basic\_RAG.ipynb

├── Advanced-Rag/

│   └── Advanced\_RAG.ipynb

├── requirements-basic.txt

├── requirements-advanced.txt

├── README.md

└── .gitignore

```



\## Implementations



\### 1. Basic RAG



A fundamental RAG pipeline designed to answer questions using a collection of academic PDF documents.



\*\*Main components:\*\*

\- PDF text extraction using PyMuPDF.

\- Fixed-size overlapping text chunking.

\- Multilingual embeddings using Sentence Transformers.

\- Dense vector retrieval using FAISS.

\- Answer generation using Qwen2.5-3B-Instruct.

\- Interactive question-answering interface using Gradio.



\### 2. Advanced RAG



An enhanced RAG pipeline introducing more sophisticated document processing and retrieval techniques.



\*\*Main components:\*\*

\- Layout-aware PDF extraction using PyMuPDF4LLM.

\- Tesseract OCR fallback for scanned pages.

\- Heading-aware semantic chunking.

\- Dense retrieval using BGE embeddings and FAISS.

\- Sparse retrieval using BM25.

\- Hybrid retrieval with Reciprocal Rank Fusion (RRF).

\- Cross-Encoder reranking using BGE.

\- Query rewriting using Qwen2.5-3B-Instruct.

\- Retrieval evaluation using Precision@K, Recall@K, MRR and Hit@K.

\- Interactive Gradio interface.



\## Technologies



Python, PyTorch, Hugging Face Transformers, Sentence Transformers, FAISS, BM25, PyMuPDF, Tesseract OCR, Gradio and Pandas.



\## Requirements



Each implementation has its own requirements file:



\- `requirements-basic.txt`

\- `requirements-advanced.txt`



The advanced implementation additionally requires the Tesseract OCR system executable.



\## Running the Notebooks



The notebooks are designed to run in Google Colab.



1\. Open the desired notebook in Google Colab.

2\. Select a GPU runtime for accelerated model inference.

3\. Upload your PDF documents to the expected `/content/documents` directory.

4\. Execute the notebook cells in order.



The language models and embedding models are downloaded from Hugging Face when needed.



\## Author



\*\*Mohamed El Hocine Goussas\*\*



AI Engineering Student | Algeria

