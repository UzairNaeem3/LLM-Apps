# Crime and Punishment Summarization

## Overview

This repository contains scripts for summarizing the classic novel "Crime and Punishment" by Fyodor Dostoevsky using natural language processing techniques.

## Files

### Pdf_Summarization.ipynb

In this notebook:
- The book is loaded and divided into its parts.
- Summaries for each part are generated. Note that due to the API key limitation, summaries for only the first 3 parts were successfully generated.
- Both Claude and GPT models were tested, with Claude used for parts of the book due to its 100k tokens limit compared to GPT's 16k limit.

### test.ipynb

This notebook is for testing purposes. It includes:
- Loading the book.
- Creating clusters of the book's documents.
- Utilizing a clustering approach by creating embeddings to identify the document that best describes the book. This approach aims to overcome token limit problems.

## Note

The Pdf file file contains summaries for the first 3 parts of the book. This limitation is due to the API key reaching its limit.

## Installation

1. Ensure you have Python installed on your system. If not, download and install it from [python.org](https://www.python.org/).

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'


## Install the required packages using pip:
pip install -r requirements.txt

## Configuration
1. **Create a file named `.env` in the project root and add your API key:**
   ```plaintext
   API_KEY=your_api_key_here

Replace your_api_key_here with the API key you obtained.

## Usage

1. Open the Jupyter Notebook Pdf_Summarization.ipynb using Jupyter or any compatible notebook viewer.
2. Run the notebook cells sequentially to execute the summarization script.
3. Review the output for the summarized content of "Crime and Punishment."

## Note

