# SplitDocument-QA

# PDF Split, Analyze, and Question with Azure and OpenAI

This repository contains a Python script to split a PDF into smaller parts, analyze each part using Azure Document Intelligence, and query the content using OpenAI's GPT-based API. If no answers are found in the document, the system will clearly indicate this.

## Features

1. **PDF Splitting**: The script splits a large PDF file into smaller parts for processing.
2. **Azure Document Intelligence Analysis**: Each split document is analyzed to extract its content in Markdown format.
3. **OpenAI Questioning**: The extracted content is sent to OpenAI's GPT-based API to answer a user-provided question.
4. **Response Combination**: Responses from all document parts are combined into a single summary.
5. **Error Handling**: If no part contains the answer, the system will respond with "No answers were found in the document."

## Requirements

### Python Packages
- `PyPDF2`: For splitting PDF files.
- `requests`: For making API requests to OpenAI.
- `azure-core` and `azure-ai-documentintelligence`: For interacting with Azure Document Intelligence.

Install these dependencies using pip:
```bash
pip install PyPDF2 requests azure-core azure-ai-documentintelligence
