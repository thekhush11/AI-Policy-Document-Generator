# AI Policy Document Generator

## Overview

The **AI Policy Document Generator** is a web-based tool that generates detailed policy documents automatically based on user input. Users can specify the domain, region, scope, and tone to generate professional policies that can be downloaded as `.docx`.

## Features

- Generate professional policy documents automatically
- Customizable inputs: domain, region, scope, tone
- Download the generated policy as `.docx`
- Uses Hugging Face models (Google/Mistral) for AI text generation

## Installation

1. Clone the repository:

```bash
git clone "https://github.com/thekhush11/AI-Policy-Document-Generator"
```

2. Create a virtual environment and activate:
   python -m venv venv

# Windows

venv\Scripts\activate

# macOS/Linux

source venv/bin/activate

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Set Hugging Face API token in .env:

```
HF_TOKEN=your_huggingface_token
MODEL_NAME=google/flan-t5-small
```

5. Download the AI model:
   python backend/scripts/download_model.py

6. Run the Project

7. Start the backend API:
   uvicorn backend.main:app --reload
   Open index.html in your browser and use the form to generate policy documents.

8. Usage
   Open frontend HTML (index.html)
   Fill in the form with domain, region, scope, and tone
   Click "Generate" to get the policy
   Download .docx if needed

9. Dependencies
   Python 3.11+
   FastAPI
   Uvicorn
   Hugging Face Transformers
   python-docx

10. License
    Educational and research purposes only.
