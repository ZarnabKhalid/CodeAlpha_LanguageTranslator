# CodeAlpha_LanguageTranslator

A **Language Translation Tool** with a simple web interface built using Streamlit.

Built as **Task 1: Language Translation Tool** of the CodeAlpha Artificial Intelligence Internship.

## Features

- Enter text and choose the **source** and **target** language
- **Auto detect** option for the source language
- Supports all languages available in Google Translate
- Translated text is displayed clearly on screen
- **Copy button:** the translation is shown in a code box with a built-in copy icon
- **Text-to-speech:** listen to the translated text (using gTTS)
- **Reliable translation:** automatic retries (up to 3 times) with Google Translate, and **MyMemory** as a backup service
- Friendly messages for empty input, failed translation and unsupported audio languages

## How it works

1. The list of supported languages is loaded from Google Translate.
2. The user types text and selects the source and target languages.
3. The text is sent to Google Translate through the `deep-translator` library (retried up to 3 times; MyMemory is used as a backup).
4. The translated text is displayed on screen.
5. An audio version of the translation is generated with `gTTS` and can be played in the browser.

## Tech stack

- Python 3
- Streamlit (user interface)
- deep-translator (Google Translate and MyMemory)
- gTTS (text-to-speech)

## Installation

```bash
pip install streamlit deep-translator gTTS
```

## Usage

```bash
streamlit run app.py
```

The app opens in your browser at `http://localhost:8501`.

Note: replace `app.py` with the name of the main Python file if it is different.

## Author

Zarnab Khalid - CodeAlpha AI Intern
