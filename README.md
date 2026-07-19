# 🎙️ AI Voice Translator

A sleek, dark-themed voice translation web app that lets you speak in one language and get an instant translation in another — right in your browser, no backend required.

![Tech](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Tech](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Tech](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## ✨ Features

- 🎤 **Voice Input** — Speak naturally using your browser's built-in speech recognition
- ⌨️ **Manual Text Input** — Type instead of (or alongside) speaking, as a fallback when mic access is blocked
- 🌍 **Multi-language Support** — English, Urdu, Spanish, French, German, Arabic, Hindi, and Chinese
- 🔄 **Language Swap** — One click to swap source and target languages
- 🔊 **Text-to-Speech Playback** — Listen to the translated text out loud
- 📋 **Copy to Clipboard** — Copy the translation with one click
- ❤️ **Save/Like** — Mark translations you want to remember
- 🌗 **Dark / Light Mode Toggle**
- 📱 **Fully Responsive** — Works on desktop and mobile
- 🔁 **Dual Translation API Fallback** — Automatically switches to a backup service if the primary one fails

## Screenshot
<img width="935" height="427" alt="image" src="https://github.com/user-attachments/assets/1cd2c759-03c5-4030-abb4-c1d37887f119" />

## 🛠️ Tech Stack

**Frontend**
- HTML5
- CSS3 (Vanilla — no framework, custom properties, flexbox/grid, keyframe animations)
- JavaScript (ES6+, Vanilla — no framework)

**Browser APIs**
- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) — Speech-to-text
- [SpeechSynthesis API](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis) — Text-to-speech
- [Clipboard API](https://developer.mozilla.org/en-US/docs/Web/API/Clipboard) — Copy functionality

**Translation Services (free, no API key required)**
- Google Translate (unofficial public endpoint) — primary
- [MyMemory Translation API](https://mymemory.translated.net/) — fallback

**Architecture**
- 100% client-side — no backend, no database, no build tools
- Single self-contained `index.html` file

## 🚀 Getting Started

### Option 1: Just open it
Simply open `index.html` in a modern browser (Chrome or Edge recommended for full Speech Recognition support).

### Option 2: Run locally with a server
```bash
git clone https://github.com/safiadeveloper/ai-voice-translator.git
cd ai-voice-translator
# Using Python
python -m http.server 8000
# Then visit http://localhost:8000
```

> **Note:** Speech recognition requires microphone permission and works best over `https://` or `localhost`. If mic access is blocked (common in some embedded/preview environments), use the manual text input box instead.

## 📖 How to Use

1. Select your **source language** (FROM) and **target language** (TO)
2. Tap the **microphone** and speak, or type directly into the text box
3. Click **Translate**
4. View the translation, listen to it, copy it, or save it with ❤️

## 🌐 Browser Compatibility

| Feature | Chrome | Edge | Safari | Firefox |
|---|---|---|---|---|
| Speech Recognition | ✅ | ✅ | ⚠️ Limited | ❌ |
| Text-to-Speech | ✅ | ✅ | ✅ | ✅ |
| Manual Text Input / Translation | ✅ | ✅ | ✅ | ✅ |

## 📂 Project Structure

```
ai-voice-translator/
├── index.html      # Complete app (HTML + CSS + JS in one file)
└── README.md
```

## 🗺️ Roadmap

- [ ] Add conversation history / saved translations panel
- [ ] Migrate to a FastAPI backend with a paid translation API (DeepL / Azure Translator) for higher accuracy
- [ ] Add more languages
- [ ] Offline mode with cached phrases

## 👤 Author

**Safia Bibi**
- GitHub: [@safiadeveloper](https://github.com/safiadeveloper)
- LinkedIn: [safia-developer](https://linkedin.com/in/safia-developer)
- Portfolio: [safiabibiportfolio.site](https://safiabibiportfolio.site)
- Email: safia34740@gmail.com

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ If you found this project useful, consider giving it a star on GitHub!
