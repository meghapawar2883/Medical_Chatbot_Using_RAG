Medical Chatbot Using Retrieval-Augmented Generation (RAG)
This repository contains the implementation of a Medical Chatbot that leverages Retrieval-Augmented Generation (RAG) to answer medical queries accurately. The chatbot combines document retrieval with a Large Language Model (LLM) to provide contextually accurate and truthful answers. It uses PDF-based medical literature as a knowledge source.

Features
PDF Document Parsing: Automatically loads and processes PDF documents as the knowledge base.
Text Chunking: Splits documents into manageable chunks for better contextual understanding.
Vector Embeddings: Creates dense vector embeddings of text using the PubMedBERT model for semantic similarity.
Similarity Search: Retrieves relevant chunks based on user queries.
LLM Integration: Uses LLaMA-based models to generate responses informed by retrieved context.
Interactive Query Handling: Allows real-time user queries with accurate answers.
Technologies Used
Python: Programming language.
LangChain: Framework for combining language models with retrieval systems.
SentenceTransformers: Library for creating embeddings.
ChromaDB: Vector database for storing and retrieving document embeddings.
LLaMA-CPP: LLM integration for response generation.
PyPDF: Library for handling PDF document parsing.
Project Workflow
1. Load Documents
PDFs are parsed and converted into text using PyPDF. The documents are loaded from a directory specified by the user.

2. Text Chunking
The text is split into smaller chunks to ensure better embedding performance. Each chunk is 300 characters long with an overlap of 50 characters.

3. Embedding Creation
Chunks are embedded using the PubMedBERT model via SentenceTransformers to create meaningful vector representations.

4. Vector Store
All embeddings are stored in ChromaDB, enabling fast similarity-based retrieval.

5. Query Processing
User queries trigger a similarity search to fetch the most relevant chunks from the vector store. The retrieved chunks are passed to the LLM for context-aware response generation.

6. Response Generation
The LLaMA-based model processes the query and retrieved context to provide accurate answers.

