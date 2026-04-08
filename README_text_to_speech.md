# Text-to-Speech with Python 🔊
### Multilingual Speech Synthesis using Google Text-to-Speech (gTTS)

A GenAI audio project that converts text into natural-sounding speech using **Google's Text-to-Speech API** — supporting multiple languages, customizable speed, and audio file export.

---

## Overview

Text-to-Speech (TTS) is a core technology powering voice assistants, audiobooks, accessibility tools, and conversational AI. This project demonstrates how to build a complete TTS pipeline using Python's gTTS library — converting any text into spoken `.mp3` audio in seconds, across multiple languages.

---

## Features

- 🌍 **Multilingual support** — English, Turkish, Turkmen, and 30+ languages
- ⚡ **Adjustable speed** — normal and slow speech modes
- 📁 **Audio file export** — save output as `.mp3`
- 📄 **Text file input** — convert entire documents to speech
- 🎧 **Jupyter playback** — listen directly in the notebook
- 🔤 **Custom text pre-processing** — handles abbreviations, decimals, punctuation

---

## How it works

```
Input Text → gTTS object (language, speed settings)
→ Google TTS API → .mp3 Audio File → Playback
```

1. **Install gTTS** — Google's cloud TTS engine wrapper
2. **Define text & language** — any string, any supported language code
3. **Create gTTS object** — specify language, speed, regional accent (tld)
4. **Save to mp3** — exports audio file locally
5. **Play audio** — IPython display or any media player

---

## Sample output

```python
# English
text = "Hello! Welcome to the Text to Speech conversion tutorial."
language = 'en'
→ Output: natural English speech audio ✅

# Turkmen (via Turkish TTS engine)
text = "Men gyzym yene bir sagatdan gelyar."
language = 'tr'
→ Output: Turkmen/Turkish speech audio ✅
```

---

## Languages demonstrated

| Language | Code | Notes |
|----------|------|-------|
| English | `en` | Default, high quality |
| Turkish | `tr` | Also used for Turkmen text |
| 30+ others | various | Full list via `tts_langs()` |

---

## Tech stack

| Tool | Purpose |
|------|---------|
| gTTS (Google Text-to-Speech) | Core TTS engine |
| IPython.display | Audio playback in Jupyter |
| playsound | Audio playback in local environment |
| Python | Core language |

---

## How to run

```bash
# Install dependencies
pip install gTTS playsound

# Run the notebook
jupyter notebook Text_To_Speech.ipynb
```

> Works in both local Jupyter and Google Colab environments.

---

## Key concepts demonstrated

- **Text-to-Speech synthesis** — converting written text to natural audio
- **Multilingual TTS** — language code selection and cross-language support
- **Google TTS API integration** — cloud-based speech synthesis
- **Audio file management** — saving and playing `.mp3` output
- **Language detection** — programmatically listing all supported languages

---

## Related project

🔗 [Speech-to-Text](https://github.com/Atash22/speech-to-text-python) — the reverse pipeline: converting spoken audio back into text

---

## Author

**Atageldi Kakabayev** — AI/ML Developer | GenAI · Speech AI · NLP  
[LinkedIn](https://linkedin.com/in/atageldi-kakabayev) · [GitHub](https://github.com/Atash22)
