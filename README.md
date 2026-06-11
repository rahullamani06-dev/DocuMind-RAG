# 📚 DocuMind RAG: Intelligent Document Question Answering System

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![FAISS](https://img.shields.io/badge/FAISS-Vector%20Database-green)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![NLP](https://img.shields.io/badge/NLP-RAG-orange)

## 🚀 Overview

DocuMind RAG is an intelligent document question-answering system developed as part of the **NVIDIA H200 Summer Internship Program 2026** at Presidency University.

The system enables users to upload PDF documents such as research papers, reports, manuals, academic notes, and technical documents. Using **Retrieval-Augmented Generation (RAG)**, the application retrieves relevant information from the uploaded document and generates context-aware answers along with source citations.

Unlike traditional keyword search systems, DocuMind RAG uses semantic search and transformer-based language models to understand the meaning of user queries and provide accurate responses.

---

## 🎯 Problem Statement

Large PDF documents often contain valuable information, but manually searching through hundreds of pages is time-consuming and inefficient.

Traditional keyword-based search systems:

* Depend on exact word matches
* Lack contextual understanding
* Cannot generate direct answers

DocuMind RAG addresses these challenges by combining semantic retrieval with language generation.

---

## ✨ Features

* 📄 PDF Upload Support
* 🔍 Automatic Text Extraction
* ✂️ Text Chunking with Overlap
* 🧠 Semantic Embedding Generation
* 📊 FAISS Vector Database
* 🤖 Retrieval-Augmented Generation (RAG)
* 💬 Document Question Answering
* 📚 Source Page Citations
* 🌐 Interactive Gradio Interface
* ⚡ Google Colab Compatible

---

## 🏗️ System Architecture

```text
User Uploads PDF
        │
        ▼
PDF Text Extraction
        │
        ▼
Text Cleaning
        │
        ▼
Chunking
        │
        ▼
Embedding Generation
        │
        ▼
FAISS Vector Database
        │
        ▼
User Question
        │
        ▼
Query Embedding
        │
        ▼
Similarity Search
        │
        ▼
Context Retrieval
        │
        ▼
FLAN-T5 Answer Generation
        │
        ▼
Answer + Source Citations
```

---

## ⚙️ Technology Stack

| Technology                | Purpose                 |
| ------------------------- | ----------------------- |
| Python                    | Programming Language    |
| PyTorch                   | Deep Learning Framework |
| Hugging Face Transformers | Language Models         |
| Sentence Transformers     | Embedding Generation    |
| all-MiniLM-L6-v2          | Semantic Embeddings     |
| FLAN-T5                   | Answer Generation       |
| FAISS                     | Vector Database         |
| PyMuPDF                   | PDF Processing          |
| Gradio                    | User Interface          |
| Google Colab              | Development Environment |

---

## 🔄 Project Workflow

### Step 1: PDF Upload

The user uploads a PDF document through the Gradio interface.

### Step 2: Text Extraction

Text is extracted page by page using PyMuPDF.

### Step 3: Text Chunking

The extracted content is divided into smaller overlapping chunks for efficient retrieval.

### Step 4: Embedding Generation

Each chunk is converted into vector embeddings using the all-MiniLM-L6-v2 Sentence Transformer model.

### Step 5: Vector Storage

Embeddings are stored inside a FAISS vector database.

### Step 6: User Query Processing

The user enters a question related to the uploaded document.

### Step 7: Similarity Search

The query embedding is compared with document embeddings to retrieve relevant chunks.

### Step 8: Answer Generation

Retrieved chunks are provided as context to the FLAN-T5 language model.

### Step 9: Citation Generation

Source page numbers are displayed alongside generated answers.

---

## 📂 Project Structure

```text
DocuMind-RAG/
│
├── README.md
├── requirements.txt
├── app.py
│
├── modules/
│   ├── pdf_processor.py
│   ├── chunking.py
│   ├── embeddings.py
│   ├── vector_store.py
│   ├── retrieval.py
│   ├── generator.py
│   └── citation.py
│
├── screenshots/
│
├── report/
│
└── presentation/
```

---

## 🛠️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/DocuMind-RAG.git

cd DocuMind-RAG
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

Launch the application:

```bash
python app.py
```

Or run the notebook in Google Colab and launch the Gradio interface.

---

## ❓ Sample Questions

Try asking:

* How many credits are awarded?
* What is the duration of the internship program?
* What hardware is used?
* What are the prerequisites?
* What project tracks are available?

---

## 📈 Results

The system successfully:

* Processes PDF documents
* Generates semantic embeddings
* Performs vector similarity search
* Retrieves relevant document content
* Generates context-aware answers
* Displays source page citations

The application was tested on multiple PDF documents including internship guides, technical reports, academic notes, and research papers.

---

## 🔮 Future Scope

Potential future enhancements include:

* Multi-document support
* OCR for scanned PDFs
* Multilingual document understanding
* Larger language models
* Cloud deployment
* Conversational memory

---

## 🎓 Learning Outcomes

Through this project, the following concepts were implemented and understood:

* Natural Language Processing (NLP)
* Retrieval-Augmented Generation (RAG)
* Transformer Models
* Sentence Embeddings
* Vector Databases
* Semantic Search
* Question Answering Systems
* Gradio Application Development

---

## 👨‍💻 Team Members

* Rahul I Lamani
* Kartik Naik
* Sagar Jain
* Yuvaraj Nanganuri

Department of Computer Science and Technology

Presidency University

---

## 🏆 NVIDIA H200 Summer Internship Program 2026

Track B — Natural Language Processing (NLP)

Project Theme:

**Question Answering System using Retrieval-Augmented Generation (RAG)**

---

## 📄 License

This project is licensed under the MIT License.
