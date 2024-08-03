# Acessing-Particular-Topics-from-pdf-using-Llama3-model

# RAG with Llama3 and PDF Extraction

This project demonstrates how to create a Retrieval-Augmented Generation (RAG) pipeline using the Ollama Llama3 model and PyMuPDF for extracting text from a PDF. The text is split into chunks, embedded, and stored in a vector store to enable efficient retrieval and context-based question answering.

## Requirements

To run this project, you'll need to install the following Python packages:

- `fitz` (PyMuPDF)
- `ollama`
- `langchain`
- `langchain_community`

You can install these packages using pip:

```bash
pip install pymupdf ollama langchain langchain_community
