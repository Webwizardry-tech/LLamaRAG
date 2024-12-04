# README

## Project: Python Knowledge Retrieval System with LangChain

This project builds a question-answering system using LangChain and related tools to process a Python-related PDF, create embeddings for efficient search, and construct a pipeline for retrieving answers from the document.

---

## Table of Contents

1. [Overview](#overview)  
2. [Features](#features)  
3. [Requirements](#requirements)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Components](#components)  
7. [Example Query](#example-query)  
8. [Acknowledgements](#acknowledgements)  

---

## Overview

The system is designed to:  
1. Load a PDF document (`Learning_Python.pdf`) containing information about Python programming.  
2. Split the document into manageable text chunks.  
3. Create embeddings for the chunks using an Ollama embedding model.  
4. Store the embeddings in a local Chroma database.  
5. Retrieve relevant context for a given query and provide detailed answers using a prompt-powered LLM.

---

## Features

- **PDF Parsing**: Converts a Python-related PDF into usable text chunks.  
- **Embeddings**: Generates embeddings using the `nomic-embed-text` model for semantic search.  
- **Vector Store**: Uses Chroma for efficient local storage and retrieval.  
- **Prompt Engineering**: A predefined prompt guides the assistant to provide clear and detailed answers.  
- **Question-Answering Pipeline**: Uses a retrieval-augmented generation (RAG) setup to answer queries.

---

## Requirements

- Python 3.8 or later
- Required libraries:
  - `langchain`
  - `langchain-ollama`
  - `langchain-chroma`
  - `langchain-core`
  - `pypdf`
  - `chromadb`

---

## Installation

1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
