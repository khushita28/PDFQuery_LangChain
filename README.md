PDF Document Question Answering System
This project builds a PDF Document Question Answering system using Langchain, Astra DB (Cassandra), and a Vector Database to efficiently handle and answer questions based on PDF documents. The system extracts text from PDF files, generates embeddings for searchability, stores these embeddings in Astra DB, and retrieves relevant sections to answer queries with a Language Model.

Project Overview
  1)Text Extraction: Parses and extracts text from PDF documents.
  2)Embeddings Generation: Converts text into vector embeddings to facilitate semantic search.
  3)Vector Storage in Astra DB: Stores embeddings in Cassandra’s Astra DB with a vector index for efficient retrieval.
  4)Relevant Section Retrieval: Uses vector similarity to find document sections that align with a given question.
  5)LLM-Based Question Answering: Generates answers based on the content of retrieved sections, using Langchain’s LLM capabilities.

Prerequisites
  Python 3.7+
  Astra DB Account with a keyspace configured for vector storage.
  Google Colab or Local Development Environment

Configuration
  Astra DB Setup: Configure Astra DB credentials and endpoint in the project.
  Langchain API Keys: Set up API keys for the embedding and Language Model functionalities.

Example Workflow
  Load PDF Documents: Add documents to the documents/ folder.
  Process and Store: Run the script to extract, embed, and store document content.
  Query and Answer: Input questions, and the system retrieves and interprets relevant text segments to generate answers.

Future Improvements
  Enhanced PDF Preprocessing: Incorporate support for complex document structures.
  Multi-Document Search: Enable search across multiple documents in the system.
  Caching Mechanism: Implement caching for frequently accessed documents and embeddings.

License
This project is licensed under the MIT License.
