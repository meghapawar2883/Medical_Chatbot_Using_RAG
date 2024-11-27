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
