# Aura — Mental Health Companion Chatbot

**IBM Edunet SkillsBuild project.** Students face high levels of stress,
anxiety, and loneliness but often hesitate to approach professional
counselors. Aura is a safe, AI-driven chatbot that detects user mood through
sentiment analysis and responds with empathetic, motivational messages and
relaxation tips to support student mental well-being.

## Features

- Empathetic conversational companion ("Aura" persona via system prompt)
- Mood detection through sentiment analysis
- Motivational responses + relaxation tips
- Clean Streamlit chat UI

## Tech Stack

- **Python**, **Streamlit**
- **Google Gemini API** (`google-generativeai`) — primary LLM
- **Hugging Face** (`hf_client.py`) — sentiment/auxiliary models
- `requests`

## Getting Started

```bash
pip install -r IBM_Project/requirements.txt
```

Add your Gemini API key to Streamlit secrets (`.streamlit/secrets.toml`):

```toml
GEMINI_API_KEY = "your-key-here"
```

Then run:

```bash
streamlit run IBM_Project/app_old.py
```

> Never commit API keys. The app reads the key from Streamlit secrets —
> keep it out of git.

## Project Structure

```
IBM_Project/
  app_old.py          # Streamlit app ("Aura")
  gemini_client.py    # Gemini API client
  hf_client.py        # Hugging Face client
  requirements.txt
```

## Author

Kazi Nafis Nawaz
