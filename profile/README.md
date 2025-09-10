
---

# 🤖 Zentry AI Assistant

![GitHub repo size](https://img.shields.io/github/repo-size/Zentry-org/.github)
![GitHub contributors](https://img.shields.io/github/contributors/Zentry-org/.github)
![GitHub last commit](https://img.shields.io/github/last-commit/Zentry-org/.github)
![Issues](https://img.shields.io/github/issues/Zentry-org/.github)
![License](https://img.shields.io/github/license/Zentry-org/.github)

> 🚀 An open-source, real-time AI Voice Assistant for intelligent, human-like conversations – built to serve institutions, automate tasks, and adapt to your context.

---

## 📝 Abstract

**Zentry AI Assistant** is a **modular and real-time voice AI system** designed for **telephony and institutional automation**. It combines **high-accuracy speech-to-text (STT)**, **reasoning with lightweight LLMs**, and **natural speech synthesis (TTS)** to create seamless human-like conversations in local languages.

Built around **FreeSWITCH** for call control, **CTranslate2-optimized Whisper** for efficient transcription, and **Phi-3 Mini with RAG** for factual reasoning, Zentry emphasizes **speed, accuracy, and locality**. The assistant is extendable with **Meta MMS multilingual models** for broader language coverage, enabling use in education, healthcare, and enterprise environments.

---

## ✨ Key Features

* 🎙️ **STT (Malayalam + English)** using **Whisper-medium CTranslate2**
* 🧩 **Reasoning & RAG** with **Phi-3 Mini** (low-latency + factual)
* 🌐 **Multilingual extension** via **Meta MMS** speech models
* ☎️ **FreeSWITCH SIP integration** for call routing + telephony
* 💬 **Dynamic response generation**
* 📦 **Lightweight + fully local** (edge-device deployable)
* 🔌 **API-first** for easy integration with external systems

---

## 🛠️ Tech Stack

| Component        | Tech / Tool                                  |
| ---------------- | -------------------------------------------- |
| Speech-to-Text   | Whisper-medium (CTranslate2 runtime)         |
| NLP / Reasoning  | Phi-3 Mini + RAG pipeline                    |
| Multilingual STT | Meta MMS (Vineel’s fine-tuned speech models) |
| Voice I/O        | FreeSWITCH + Linphone SIP                    |
| Backend          | Python (FastAPI / Flask optional)            |
| Orchestration    | Docker, Supervisor                           |
| Real-Time Engine | Asyncio + WebSockets                         |

---

## 🚀 Quick Start

### 🔧 Prerequisites

* Python 3.9+
* FFmpeg
* CTranslate2 + Whisper model
* FreeSWITCH running with SIP endpoints
* `linphonec` or any SIP client

```bash
git clone https://github.com/Zentry-org/.github.git
cd zentry-ai-assistant

# Create a virtual environment
python3 -m venv venv && source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Download and optimize Whisper model
python setup_model.py

# Start the assistant
python run_assistant.py
```

---

## 🔁 Architecture

```text
[Caller] ↔ [FreeSWITCH] ↔ [Linphone] ↔ [VoiceBot.py]
                               ↓
                 [STT: Whisper (CTranslate2)]
                               ↓
            [LLM: Phi-3 Mini + Retrieval (RAG)]
                               ↓
             [TTS / Playback with future module]
```

---

## 🧪 Use Cases

* 🎓 College reception desk voice assistant
* 📞 Automated helpline support
* 🏥 Healthcare triage voicebot
* 🌐 Local-language assistants (Malayalam, Tamil, Hindi, etc.)

---

## 🛤️ Roadmap

* [x] STT with Whisper (CTranslate2 optimized)
* [x] FreeSWITCH SIP integration
* [ ] MMS Meta integration for multilingual STT
* [ ] TTS Module (Indic-TTS / Coqui extension)
* [ ] Phi-3 Mini RAG optimization for factual answers
* [ ] Conversation monitoring dashboard
* [ ] Deployable builds for Raspberry Pi / edge

---

## 💡 Contributing

We welcome your contributions!

```bash
# Fork the repo, make changes, and submit a PR 🚀
```

Check [CONTRIBUTING.md](https://github.com/Zentry-org/.github/blob/main/CONTRIBUTING.md) before submitting.

---

## 📜 License

MIT License – see [LICENSE](LICENSE)

---

## 🌐 Connect with Us

* Organization: [Zentry](https://github.com/Zentry-org)
* Developers: [Habel Shaji](https://github.com/Habel2005) | [Lino Tom](https://github.com/LinoTom)
* Still Doubt?: Some DevNotes [Notion](https://ruddy-manchego-5eb.notion.site/Zentry-Ai-24f8e847267180a18c3dd96f3b8d59f9)

---

> *"The future of voice is local, inclusive, and intelligent. Let's build it together."* – Team Zentry

---

Do you want me to also add a **Demo / Benchmark section** (with response time goals like <2s, WER numbers for Malayalam STT) so people see your project’s performance metrics?
