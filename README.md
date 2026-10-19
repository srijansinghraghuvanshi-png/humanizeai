# HumanizeAI ✍️

An AI-powered writing assistant built with Python and Streamlit. HumanizeAI helps improve grammar, clarity, flow, and readability while aiming to preserve the author's meaning.

<p align="left">
  <a href="https://humanizeai-srijan-singh-raghuvanshi.streamlit.app/"><strong>🚀 Try the live app</strong></a>
  ·
  <a href="https://github.com/srijansinghraghuvanshi-png/humanizeai"><strong>View source code</strong></a>
</p>

## Features

- **Two writing modes:** Academic / Research and Blog / General
- **Five writing tones:** Natural and clear, Professional, Simple English, Concise, and Friendly
- **Side-by-side workspace:** Keep the original draft visible while reviewing the revised text
- **Editor notes:** See notes returned by the model
- **Download results:** Save the revised text and editor notes as a `.txt` file
- **Cloud AI inference:** Uses the Groq API
- **Responsive interface:** Built with Streamlit and custom CSS

## Tech stack

- Python
- Streamlit
- Requests
- Groq API (OpenAI-compatible chat completions endpoint)

## Try it online

1. Open the [HumanizeAI live app](https://humanizeai-srijan-singh-raghuvanshi.streamlit.app/).
2. Choose a writing goal and tone from the sidebar.
3. Paste a draft into the left text area.
4. Select **Improve my writing**.
5. Review the revised text and editor notes before using the result.
6. Download the result as a text file if needed.

## Run locally

### Requirements

- Python 3.10 or newer recommended
- A Groq account and API key

### Setup

1. Clone this repository:

   ```powershell
   git clone https://github.com/srijansinghraghuvanshi-png/humanizeai.git
   cd humanizeai
   ```

2. Create and activate a virtual environment:

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

3. Install dependencies:

   ```powershell
   python -m pip install -r requirements.txt
   ```

4. Add your Groq API key to Streamlit secrets. Create a file at `.streamlit/secrets.toml` with this content:

   ```toml
   GROQ_API_KEY = "paste_your_own_key_here"
   ```

   Replace the example value with your own key. **Never commit this file or publish your API key.** The repository's `.gitignore` excludes local secrets.

5. Start the app:

   ```powershell
   python -m streamlit run app.py
   ```

6. Open the local URL shown in the terminal, usually `http://localhost:8501`.

## Configuration and privacy

- The app reads `GROQ_API_KEY` from Streamlit secrets.
- Writing submitted for improvement is sent to the configured Groq API for processing. Do not paste passwords, private records, or other sensitive information.
- API availability, supported models, rate limits, and free-tier quotas depend on the provider and may change.
- Never store API keys in source code, screenshots, or public commits.

## Responsible use

HumanizeAI is a writing aid, not a substitute for your own judgment. Review every revision, verify factual claims and citations independently, and make sure the final work reflects your own understanding. The app is not designed to evade AI-detection systems or misrepresent authorship.

## Current limitations

- Model output can contain mistakes or alter nuance; always proofread the result.
- The app requires network access to reach Groq.
- Free API usage may be subject to rate limits or quotas.

## License

No license has been selected yet. Unless a license is added, all rights are reserved.
