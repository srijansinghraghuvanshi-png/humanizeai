# Manual Testing

This document records basic manual checks for HumanizeAI. These are functional spot checks, not a formal benchmark or a guarantee of writing quality.

## Test environment

- Deployed Streamlit application
- Writing goal: Academic / Research
- Writing tone: Natural and clear
- AI provider: Groq API
- Model configured in the application: `openai/gpt-oss-20b`

## Test cases

| Test | Input | Expected behavior | Observed result |
|---|---|---|---|
| Text refinement | A short paragraph about how AI changes writing | Improve phrasing and readability while preserving the meaning | The app returned a revised paragraph with wording changes |
| Grammar correction | A paragraph containing subject-verb agreement and verb-form errors | Correct clear grammar mistakes without changing the core meaning | The app corrected examples such as “AI are” to “AI is” and “people works” to “people work” |

## Review checklist

Before using or publishing generated text:

- Compare the revision with the original.
- Confirm the original meaning, qualifications, and tone are preserved.
- Verify factual claims, names, quotations, and citations independently.
- Do not paste passwords, private records, or other sensitive information into the app.

## Limitations

- These are a small number of manual examples, not a representative evaluation dataset.
- Outputs can contain errors or alter nuance.
- Factual accuracy and citations are not independently verified by the app.
- Results may vary with model behavior, API availability, and provider limits.

## Running further tests

Try a variety of inputs: clean prose, grammar errors, long paragraphs, empty input, technical terminology, and text containing claims or citations. Record failures and improvements here when verified.
