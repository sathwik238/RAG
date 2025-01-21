# Retrieval-Augmented Generation (RAG) Demo

This project demonstrates the use of **Retrieval-Augmented Generation (RAG)** to build a search and query system using OpenAI and LlamaIndex. It processes documents, creates an index, and allows users to search and retrieve relevant information from their content.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)

---

## Overview

Retrieval-Augmented Generation (RAG) combines information retrieval and generative AI to provide contextual, document-based answers to queries. This project leverages RAG to build a pipeline that indexes PDF files and enables users to query them with natural language.

The demo focuses on creating an end-to-end RAG solution for indexing and querying two sample PDF documents.

---

## Dataset

### Input Files:
- Two sample PDF documents (`file1.pdf` and `file2.pdf`).
- Documents contain text that needs to be indexed and queried.

### Features:
1. **Text Extraction**:
   - Extracts text from uploaded PDF files.
2. **Index Creation**:
   - Creates a vector-based index for efficient querying.
3. **Query and Retrieval**:
   - Accepts natural language queries and generates relevant responses.

---

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - `llama-index` (LlamaIndex for indexing and retrieval)
  - `openai` (for natural language understanding)
  - `PyPDF2` (for PDF text extraction)
  - `dotenv` (for secure API key handling)
  - `tqdm` (for progress tracking)
- **Development Environment**: Jupyter Notebook


---
