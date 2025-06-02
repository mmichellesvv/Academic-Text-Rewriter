# Academic text rewriter

Repo provides a Python script for translating the contents of Excel files between different languages.

---
### Abstract

Publishing is a tricky issue when it comes to renovating and extending the original book — by adding paragraphs, text chunks, or other details. Thanks to Python and Groq Cloud, editorial audits can be automated. This repo offers a flexible tool for text rewriting with slight expansion and auto translation.

---

## Features

- **Automatic File Detection:** The script automatically detects the first Excel file in the current directory.
- **Language Translation:** Translates text from one language to another using the `translate` library.
- **Progress Indicator:** Displays a progress indicator while processing the translation.
- **Output Naming:** Saves the translated file with a prefix indicating the target language.

## Installation

To install the required libraries, run:

```bash
python 3.11.9
```
```bash
pip install -r requirements.txt
```

## Usage

1. Download the **rewrIT-er.py** file. Place it along with aimed .docx or .pdf file in the same folder. Open a terminal (Command Prompt) and navigate to this folder (cd [folder name]).
2. Run the script from the command line as follows:
```bash
python rewrIT-er.py --token [your GROQ-token] [input_file] [output_file]
```
- `from_lang`: The language code of the source language (e.g., `"ru"` for Russian).
- `to_lang`: The language code of the target language (e.g., `"uk"` for Ukrainian).

### Example

To translate an Excel file from Russian to Ukrainian:
```bash
python translate_excel.py ru uk
```

**IMPORTANT**: This script will process the **first** .xlsx file it finds in the directory. **Ensure that only one excel file you want to translate is in the folder!**

#### License

This project is licensed under the MIT License - see the MIT.md file for details.

## In-data:
<img src="https://github.com/user-attachments/assets/f4880462-4cca-4059-9a3f-a4819146463b" alt="Description of image" width="700"/>

## Out-data:
<img src="https://github.com/user-attachments/assets/c0eb7a1f-dfcd-4718-8c74-7fee61e1e210" alt="Description of image" width="700"/>


