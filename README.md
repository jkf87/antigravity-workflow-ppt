# Academic PPT Generator

This tool generates PowerPoint presentations with academic-style images using Google's Gemini API.

## Setup

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Set up your API key:
   - Copy `.env.example` to `.env`
   - Paste your Google Gemini API key into `.env` (just the key, no `API_KEY=` prefix)

## Usage

1. Prepare your slides content in `slides.json`.
2. Run the script:
   ```bash
   python generate_ppt.py
   ```
