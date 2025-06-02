# Academic Text Rewriter

This repository provides a Python script for rewriting academic texts (from `.docx` or `.pdf`) with optional expansion, using Groq Cloud's language models.

---

## Abstract

Publishing is a tricky issue when it comes to renovating and extending the original book — by adding paragraphs, text chunks, or other details. Thanks to Python and Groq Cloud, editorial audits can be automated. This repo offers a flexible tool for text rewriting with slight expansion..

---

## Features

- **Multi-format Input Support**: Automatically processes either `.docx` or `.pdf` files, depending on the file extension.
- **Chunk-wise Rewriting**: Splits input text into manageable chunks (by paragraphs in `.docx`, or reconstructed paragraph-like segments in `.pdf`) before rewriting, which helps preserve context and improves output quality.
- **Groq Cloud API Integration**: Uses Groq language models for semantic rewriting with optional content expansion.
- **Preserves Logical Structure**: Special handling of headings or section openers (e.g., lines ending with a colon) to keep text coherent across chunks.
- **Terminal-based CLI Tool**: No GUI needed; just run the script from terminal with a few parameters.
- **Automatic File Detection**: The script detects the first supported file (`.docx` or `.pdf`) in the directory if no input is explicitly provided.

---

## Usage

### API Key Creating

Go to [https://console.groq.com/keys](https://console.groq.com/keys). Log in, create an API key, copy the token, and **keep it safe**.

---

### Installation
1. Download `requirements.txt` and `rewrIT-er.py` files from this repository.
2. Place them in the **same** folder as the `.docx` or `.pdf` file you want to rewrite.
3. Open a terminal (Command Prompt or Bash) and navigate to this folder:
```bash
cd [your-folder-name]
```
4. Create a virtual environment (**optional** but recommended):
```bash
python3 -m venv venv
source venv/bin/activate        # On Unix/macOS
venv\Scripts\activate           # On Windows
```
- To install `Python 3.11.9` **if not already installed**:

```bash
winget install --id Python.Python.3.11 --source winget
```
- To install the required libraries, run:

```bash
pip install -r requirements.txt
```
- To run the script:

```bash
python rewrIT-er.py --token [your Groq-API-Key] [input_file] [output_file]
```

---

### Example

- To rewrite the content of a DOCX or PDF file:

```bash
python rewrIT-er.py --token gsk_... book_origin.docx book_copy.docx
```

**IMPORTANT**: This script will process the **first** `.docx` or `.pdf` file it finds in the directory. Ensure that only one doc/pdf file you **want** to translate is in the folder!

---

## License

This project is licensed under the MIT License - see the `MIT.md` file for details.

---

## In:
<img src="https://github.com/user-attachments/assets/062318a4-95b7-4c58-bff3-25eee9325913" alt="Description of image" width="700"/>

## Out:
```bash
- Processing 1 pages/chunks...

📄 Page 1

- Done successfuly! Head to: book_copy.docx
```
<img src="https://github.com/user-attachments/assets/f2e8cf41-1e66-403e-a255-425ac7c3c6e3" alt="Description of image" width="700"/>




