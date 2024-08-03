# Acessing-Particular-Topics-from-pdf-using-Llama3-model

# RAG with Llama3 and PDF Extraction

This project demonstrates how to create a Retrieval-Augmented Generation (RAG) pipeline using the Ollama Llama3 model and PyMuPDF for extracting text from a PDF. The text is split into chunks, embedded, and stored in a vector store to enable efficient retrieval and context-based question answering.

# Project Structure
extract_text_from_pdf(pdf_path): A function that extracts text from a PDF file and returns it as a Document object.
RecursiveCharacterTextSplitter: A utility to split the text into chunks of manageable size.
OllamaEmbeddings: A class to create embeddings for the text chunks.
Chroma: A vector store to store the embeddings for efficient retrieval.
ollama_llm(question, context): A function to call the Ollama Llama3 model with a question and context, and return the response.
rag_chain(question): A function that retrieves relevant chunks based on the question and generates a response using the Ollama Llama3 model.
get_important_facts(question): A wrapper function that calls rag_chain to get important facts based on a question.


## Requirements

To run this project, you'll need to install the following Python packages:

- `fitz` (PyMuPDF)
- `ollama`
- `langchain`
- `langchain_community`

You can install these packages using pip:

```bash
pip install pymupdf ollama langchain langchain_community

