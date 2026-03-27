# AI-Powered Smart Document Assistant using Generative AI

## Overview
This project implements an AI-powered document assistant that performs summarization, keyword extraction, and question answering on uploaded documents. The system supports multiple file formats including PDF, DOCX, and TXT, and leverages state-of-the-art transformer-based models for natural language understanding.

The application is built using Streamlit and integrates pretrained models from Hugging Face Transformers and Sentence Transformers.

---

## Problem Statement
Large documents are often difficult to analyze manually. This project aims to:

- Automatically summarize long documents
- Extract key topics and keywords
- Enable interactive question answering
- Improve productivity in document analysis

---

## Features

- Upload multiple documents (PDF, DOCX, TXT)
- Automatic text extraction and preprocessing
- Document summarization using transformer models
- Keyword extraction using KeyBERT
- Context-based question answering
- Interactive web interface using Streamlit

---

## Supported File Formats

- PDF
- DOCX
- TXT

---

## Methodology

### 1. Text Extraction
- PDF files processed using PyPDF2
- DOCX files processed using python-docx
- TXT files read directly

---

### 2. Text Preprocessing
- Removal of newline characters
- Basic cleaning and normalization

---

### 3. Summarization
- Model: facebook/bart-large-cnn
- Type: Abstractive summarization
- Generates concise summaries from long documents

---

### 4. Keyword Extraction
- Model: KeyBERT with SentenceTransformer (all-MiniLM-L6-v2)
- Extracts top keywords based on semantic similarity

---

### 5. Question Answering
- Model: distilbert-base-cased-distilled-squad
- Performs extractive QA using document context
- Returns the most relevant answer span

---

## System Architecture

1. User uploads document(s)
2. Text is extracted and cleaned
3. User selects a document
4. System provides three functionalities:
   - Summarization
   - Keyword extraction
   - Question answering

---

## Project Structure
├── app.py
├── requirements.txt
├── README.md

---

## Installation

### 1. Clone the Repository
git clone https://github.com/your-username/ai-document-assistant.git

cd ai-document-assistant

### 2. Install Dependencies
pip install -r requirements.txt

---

## Running the Application

streamlit run app.py

---

## Model Details

- Summarization Model: BART (facebook/bart-large-cnn)
- Question Answering Model: DistilBERT (SQuAD fine-tuned)
- Keyword Extraction: KeyBERT with Sentence Transformers

---

## Results

- Generates coherent summaries for long documents
- Extracts meaningful keywords reflecting document topics
- Accurately answers user queries based on document context

---

## Key Insights

- Transformer models provide strong performance for NLP tasks
- Combining multiple NLP capabilities improves usability
- Semantic embeddings enhance keyword extraction quality
- Context-aware QA enables interactive document exploration

---

## Limitations

- Performance depends on document size and quality
- Large documents may require chunking for better results
- Extractive QA may not handle complex reasoning questions
- Model inference can be computationally expensive

---

## Future Improvements

- Implement document chunking for long texts
- Add support for more file formats (HTML, CSV)
- Use advanced models (GPT-based, LLaMA)
- Deploy on cloud platforms for scalability
- Add user authentication and document history
- Improve UI with visual analytics

---

## Conclusion

This project demonstrates the integration of generative AI and NLP techniques to build a smart document assistant. It highlights how transformer models can be used to automate document understanding tasks such as summarization, keyword extraction, and question answering.

---

## Author

Sandeep S L  
MSc Data Analytics (Computational Science)  
Digital University of Kerala  

---

## License

This project is open-source and available under the MIT License.
