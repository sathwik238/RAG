# Retrieval-Augmented Generation (RAG) Demo

This repository demonstrates the use of **Retrieval-Augmented Generation (RAG)** to build advanced search and query systems using OpenAI and LlamaIndex. It includes two projects that showcase the implementation of RAG for different data types and use cases.

---

## Table of Contents

- [Overview](#overview)
- [Projects](#projects)
  - [Project 1: PDF Document Search System](#project-1-pdf-document-search-system)
  - [Project 2: Job Description Keyword Extraction System](#project-2-job-description-keyword-extraction-system)
- [Technologies Used](#technologies-used)

---

## Overview

Retrieval-Augmented Generation (RAG) combines information retrieval and generative AI to provide contextual, document-based answers to queries. This repository features two projects:

1. **PDF Document Search System**: A pipeline for indexing and querying PDF files.
2. **Job Description Keyword Extraction System**: A pipeline for extracting resume keywords from job descriptions stored in a CSV file.

Each project demonstrates an end-to-end RAG workflow, including data preprocessing, embedding calculations, similarity scoring, and OpenAI API integration.

---

## Projects

### Project 1: PDF Document Search System

This project focuses on indexing and querying PDF files using RAG.

#### Features:
1. **Text Extraction**:
   - Extracts text from uploaded PDF files (`Attention.pdf` and `YOLO.pdf`).
2. **Index Creation**:
   - Creates a vector-based index using `llama-index` for efficient querying.
3. **Query and Retrieval**:
   - Accepts natural language queries and generates relevant responses using OpenAI's GPT API.

#### Dataset:
- Input Files: Two sample PDF documents (`Attention.pdf` and `YOLO.pdf`).

#### Example Use Case:
- Query: "What is the significance of attention mechanisms?"
- Response: Contextual information retrieved from `Attention.pdf`.

---

### Project 2: Job Description Keyword Extraction System

This project focuses on extracting resume keywords from job descriptions stored in a CSV file using RAG.

#### Features:
1. **Data Loading**:
   - Loads job descriptions from a CSV file containing a `description` column.
2. **Embedding Calculation**:
   - Calculates embedding vectors for job descriptions and the job role query using OpenAI's embedding API.
3. **Similarity Scoring**:
   - Computes the dot product to rank job descriptions based on relevance to the query.
4. **Keyword Generation**:
   - Passes the top-ranked job descriptions and the query to OpenAI's GPT API to extract relevant keywords for a resume.

#### Dataset:
- Input File: `positions.csv` containing job descriptions in a `description` column.

#### Example Use Case:
- Query: "Data Scientist"
- Response: Top keywords (e.g., "Python", "Machine Learning", "SQL") extracted from the most relevant job descriptions.

---

## Technologies Used

### Programming Language:
- **Python**

### Libraries:
- `llama-index` (LlamaIndex for indexing and retrieval)
- `openai` (for natural language understanding)
- `PyPDF2` (for PDF text extraction in Project 1)
- `pandas` (for CSV processing in Project 2)
- `dotenv` (for secure API key handling)

### Development Environment:
- Jupyter Notebook

---

## How to Run

### Prerequisites:
1. Install Python (version 3.8 or later).
2. Add your OpenAI API key to a `.env` file in the root directory:
   ```plaintext
   OPENAI_API_KEY=your_api_key_here

### Steps:

1. Clone the repository:

   ```bash
   git clone <repository_url>
   cd rag-demo

2. Install dependencies:

   ```bash
   pip install -r requirements.txt

3. Run the project-specific scripts:
   ```bash
   1. job_keyword_extraction.ipynb
   2. pdf_search_system.ipynb