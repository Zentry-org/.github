# 🤖 Zentry AI Assistant

![GitHub repo size](https://img.shields.io/github/repo-size/Zentry/.github)
![GitHub contributors](https://img.shields.io/github/contributors/Zentry/.github)
![GitHub last commit](https://img.shields.io/github/last-commit/Zentry/.github)
![Issues](https://img.shields.io/github/issues/Zentry/.github)
![License](https://img.shields.io/github/license/Zentry/.github)

> 🚀 An open-source, real-time AI Voice Assistant for intelligent, human-like conversations – built to serve institutions, automate tasks, and adapt to your context.

---

## 🧠 What is Zentry AI Assistant?

**Zentry AI Assistant** is a **modular, multilingual, and real-time AI voice assistant** built to power conversational experiences in phone calls, web, or embedded environments. Designed with precision in **speech-to-text (STT), natural language processing (NLP), and dynamic response generation**, Zentry is **privacy-first, open-source**, and tuned for local languages (like Malayalam) and real-world audio conditions.

---

## ✨ Key Features

- 🎙️ **High-accuracy STT (Malayalam + English)** using fine-tuned Whisper-medium
- 🧩 **Pluggable NLU modules** (Open-source LLMs: Phi-3, Mistral, or custom)
- ☎️ **Call integration with Asterisk & Linphone**
- 💬 **Real-time response generation**
- 📦 Lightweight + runs locally
- 🌐 API-first design for integration

---

## 🛠️ Tech Stack

| Component        | Tech / Tool                                |
|------------------|---------------------------------------------|
| Speech-to-Text   | Whisper-medium (CTranslate2)                |
| NLP / Reasoning  | Phi-3 / Mistral / LLaMA / OpenRouter        |
| Voice I/O        | Asterisk + Linphone SIP                     |
| Backend          | Python (FastAPI), Flask (optional)          |
| Orchestration    | Docker, Supervisor                          |
| Real-Time Engine | WebSocket + Event Loop (asyncio)            |

---

## 📷 Demo (Coming Soon)

> Stay tuned for a complete video walkthrough and demo calls with Zentry AI in action.

---

## 🚀 Quick Start

### 🔧 Prerequisites

- Python 3.9+
- FFmpeg
- `ct2-transformers` + Whisper model
- Asterisk server running
- `linphonec` or VoIP client

---

### 🖥️ Local Setup

```bash
git clone https://github.com/Zentry/.github.git
cd zentry-ai-assistant

# Create a virtual environment
python3 -m venv venv && source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Download STT model (CTranslate2 Whisper)
python setup_model.py

# Start the assistant
python run_assistant.py
````

---

## 🔁 Architecture

```text
[Caller] ↔ [Asterisk] ↔ [Linphone] ↔ [VoiceBot.py]
                              ↓
                 [Speech-to-Text (Whisper)]
                              ↓
                  [LLM Inference / Phi-3]
                              ↓
                 [Text-to-Speech / Playback]
```

---

## 🧪 Use Cases

* 🎓 College reception desk voice assistant
* 📞 Automated helpline support
* 🏥 Healthcare triage voicebot
* 🌐 Language-specific digital assistants (Malayalam, Tamil, etc.)

---

## 🛤️ Roadmap

* [x] Malayalam STT fine-tuning
* [x] Asterisk SIP integration
* [ ] TTS Module (Tortoise or Coqui)
* [ ] Memory & context-aware responses
* [ ] Web dashboard to monitor conversations
* [ ] Deployable on Raspberry Pi / edge devices

---

## 💡 Contributing

We welcome your contributions!

```bash
# Fork the repo, make changes and submit a PR 🚀
```

Please check [CONTRIBUTING.md](https://github.com/Zentry/.github/blob/main/CONTRIBUTING.md) before submitting a pull request.

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🌐 Connect with Us

* Organization: [Zentry](https://github.com/Zentry)
* Lead Developer: [Habel Shaji](https://github.com/habelshaji)
* Questions or Ideas? [Start a Discussion](https://github.com/Zentry/.github/discussions)

---

> *"The future of voice is local, inclusive, and intelligent. Let's build it together."* – Team Zentry
