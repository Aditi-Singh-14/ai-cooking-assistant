# ai-cooking-assistant

> 🍳 A personalised AI meal suggester that learns your preferences over time — built with Python, Gradio, and the Gemini API. MLH Global Hack Week workshop.

## What it does

Answer a few questions about your kitchen setup, dietary needs, and flavour preferences. Then ask it what to cook tonight — and rate the suggestions so it gets smarter over time.

## What you'll learn

- Calling the **Gemini API** from Python
- Building a real **Gradio UI** inside a Jupyter notebook
- Reading and writing **CSV data** to build a persistent user profile
- **Prompt engineering** — how the context you give an LLM changes the quality of its output

## Getting started

### 1. Get a free Gemini API key

Go to [aistudio.google.com](https://aistudio.google.com), sign in with your Google account, and click **Get API key**. No credit card needed.

### 2. Install dependencies

```bash
pip install gradio google-generativeai pandas notebook
```

### 3. Open the notebook

```bash
jupyter notebook notebook.ipynb
```

### 4. Add your API key

When prompted in the notebook, paste your Gemini API key. It stays local and is never saved to disk.

## How it works

```
Onboarding → profile.csv → Ask what to cook → Gemini API → Suggestion → Rate it → profile.csv gets richer
```

The more you use it, the better the suggestions get.

## Structure

```
ai-cooking-assistant/
├── notebook.ipynb       ← the whole workshop, start here
├── requirements.txt     ← pip install -r requirements.txt
├── data/
│   └── profile.csv      ← created automatically on first run
└── README.md
```

## About

Built and presented live by [@TalenMud](https://github.com/TalenMud) at MLH Global Hack Week — Season Kickoff.
