# Academic text rewriter

Repo provides a Python script for translating the contents of Excel files between different languages.

---
### Abstract

Publishing is a tricky issue when it comes to renovating and extending the original book — by adding paragraphs, text chunks, or other details. Thanks to Python and Groq Cloud, editorial audits can be automated. This repo offers a flexible tool for text rewriting with slight expansion..

---

## Features

- **Automatic File Detection:** The script automatically detects the first Excel file in the current directory.
- **Language Translation:** Translates text from one language to another using the `translate` library.
- **Progress Indicator:** Displays a progress indicator while processing the translation.
- **Output Naming:** Saves the translated file with a prefix indicating the target language.

### Usage

## API Key Creating

Go to **https://console.groq.com/keys**. Log in, create key, copy number and keep it **safety**.

## Installation
1. Download the **requirements.txt** and **rewrIT-er.py** files from repo. Place it along with aimed .docx or .pdf file in the **same** folder.
2. Open a terminal (Command Prompt) and navigate to this folder (cd [folder name]).
 - To install the required libraries, run:

```bash
python 3.11.9
```
```bash
pip install -r requirements.txt
```
- To run the script:

```bash
python rewrIT-er.py --token [your Groq-API-Key] [input_file] [output_file]
```

### Example

To rewrite origin text:
```bash
python rewrIT-er.py --token gsk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx book_origin.docx book_copy.docx
```

**IMPORTANT**: This script will process the **first** .docx or .pdf file it finds in the directory. Ensure that only one doc/pdf file you **want** to translate is in the folder!

#### License

This project is licensed under the MIT License - see the MIT.md file for details.

## In-data:
<img src="https://github.com/user-attachments/assets/f4880462-4cca-4059-9a3f-a4819146463b" alt="Description of image" width="700"/>

## Out-data:
<img src="https://github.com/user-attachments/assets/c0eb7a1f-dfcd-4718-8c74-7fee61e1e210" alt="Description of image" width="700"/>


