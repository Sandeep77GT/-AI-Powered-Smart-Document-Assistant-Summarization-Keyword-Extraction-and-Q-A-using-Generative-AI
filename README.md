# -AI-Powered-Smart-Document-Assistant-Summarization-Keyword-Extraction-and-Q-A-using-Generative-AI
# 📝 AI Document Assistant

A **Streamlit-based AI-powered document assistant** that can process PDF, DOCX, and TXT files to provide **summarization, keyword extraction, and Q&A** functionalities. Built using Hugging Face Transformers, KeyBERT, and Sentence Transformers.

---

## Features

- **Summarization:** Generate concise summaries of uploaded documents using `facebook/bart-large-cnn`.
- **Keyword Extraction:** Extract the top keywords from documents using KeyBERT with Sentence Transformers.
- **Question & Answer:** Ask questions about your document content and get AI-generated answers using `distilbert-base-cased-distilled-squad`.
- **Multi-file support:** Upload multiple files and select the one you want to process.
- **Supports PDF, DOCX, and TXT files.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/AI-Document-Assistant.git
cd AI-Document-Assistant
pip install streamlit PyPDF2 python-docx transformers torch sentence-transformers keybert

Usage

Run the Streamlit app:

streamlit run app.py


Open the provided Local URL in your browser.

Upload your PDF, DOCX, or TXT files.

Use the tabs to:

Summary: Generate a summary of the document.

Keywords: Extract keywords.

Q&A: Ask questions about the document content.


Dependencies

Streamlit
PyPDF2
python-docx
Transformers
Torch
Sentence Transformers
KeyBERT


License

This project is licensed under the MIT License. See the LICENSE
 file for details.


---

If you want, I can also **provide a ready-to-use `app.py` snippet** that automatically chunks large PDFs to avoid that summarization error, so your app works out-of-the-box even for long documents like `FBL_PassItOn_Stories_Volume_1.pdf`.  

Do you want me to do that?
