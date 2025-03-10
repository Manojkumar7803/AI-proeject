# DocuQuery: AI-Powered PDF Knowledge Assistant

## Overview
DocuQuery is an AI-powered tool that allows users to upload PDF documents and ask questions based on their content. It supports three main scenarios:
1. *Price List Analyzer*: Compare prices from multiple supplier price lists.
2. *Research Paper Simplifier*: Summarize research papers and answer questions.
3. *Resume Matcher for Hiring*: Match resumes to job requirements based on skills and qualifications.

The application uses *Google Generative AI (Gemini)* for question answering and *Hugging Face embeddings* for text processing. It is built using *Streamlit* for the user interface and *LangChain* for conversational retrieval.

---

## Features
- *Upload Multiple PDFs*: Users can upload one or more PDF files for analysis.
- *Text Extraction*: Extracts text from uploaded PDFs using PyPDF2.
- *Text Chunking*: Splits the extracted text into smaller chunks for efficient processing.
- *Embeddings*: Generates embeddings using **Hugging Face's all-MiniLM-L6-v2 model**.
- *Conversational Retrieval: Uses **Google Generative AI (Gemini)* to answer user questions based on the uploaded PDFs.
- *Conversation History*: Maintains a conversation history to provide context for follow-up questions.

---

## Technologies Used
- *Streamlit*: For building the web application interface.
- *PyPDF2*: For extracting text from PDF files.
- *LangChain*: For text splitting, embeddings, and conversational retrieval.
- *Hugging Face Embeddings*: For generating text embeddings.
- *FAISS*: For efficient vector storage and retrieval.
- *Google Generative AI (Gemini)*: For generating responses to user questions.

---

## Setup Instructions

### Prerequisites
- Python 3.8 or higher.
- A Google Generative AI API key (obtained from [Google AI Studio](https://developers.generativeai.google/)).

### Installation
1. Clone the project repository or create a new project folder.
2. Create a requirements.txt file with the following content:
   ```plaintext
   streamlit
   PyPDF2
   langchain
   google-generativeai
   faiss-cpu
   langchain-community
   sentence-transformers
