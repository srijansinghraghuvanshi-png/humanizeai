# HumanizeAI ✍️

A local-first AI writing assistant built with Python, Streamlit, and Ollama. It helps revise academic and general writing for clarity, grammar, flow, and readability while aiming to preserve the author's meaning.

## Features

- Academic / Research and Blog / General writing modes
- Multiple writing tones: Natural and clear, Professional, Simple English, Concise, and Friendly
- Side-by-side draft and revised text workspace
- Editor notes and `.txt` download
- Local Ollama inference for the current desktop version
- No hosted AI API key is required for local use

## Tech stack

- Python
- Streamlit
- Requests
- Ollama with `qwen2.5:3b`

## Run locally

1. Install Python and [Ollama](https://ollama.com/).
2. Download the model:

   ```powershell
   ollama pull qwen2.5:3b
   ```

3. Open PowerShell in the project folder.
4. Create and activate a virtual environment (optional but recommended):

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

5. Install dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

6. Start the app:

   ```powershell
   python -m streamlit run app.py
   ```

7. Open the local URL shown in the terminal (usually `http://localhost:8501`).

## Deployment status

The current version calls an Ollama server at `http://localhost:11434`. That address refers to the computer running the app, so a cloud-hosted deployment needs a separate inference setup before the AI editing feature will work online. Do not publish this version as a working cloud AI app until that is configured and tested.

## Responsible use

Review every revision before using it. Verify factual claims and citations independently. HumanizeAI does not guarantee factual correctness and is not designed to evade AI detectors or misrepresent authorship.

## License

No license has been selected yet. All rights are reserved unless a license is added to this repository.
