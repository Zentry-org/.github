# 🤝 Contributing to Zentry AI Assistant

Welcome! We're thrilled you're considering contributing to **Zentry**. This assistant is open-source and community-driven — every issue you raise, line of code you write, or idea you share makes this project better.

---

## 📋 Ground Rules

Before contributing, please read these quick rules:

- Be respectful and inclusive — we value all perspectives.
- Keep your PRs focused and scoped to one problem/feature.
- Use clear commit messages (`feat:`, `fix:`, `docs:` format preferred).
- Follow the existing code style (Pythonic, clean, async-safe).
- Open an issue before submitting large features.

---

## 🛠️ How to Contribute

### 1. Clone the Repository

```bash
git clone https://github.com/Zentry/.github.git
cd zentry-ai-assistant
````

### 2. Create a Branch

```bash
git checkout -b feature/my-cool-feature
```

### 3. Make Changes

* Add code or documentation.
* Run tests (if applicable).
* Ensure no broken imports or runtime errors.

### 4. Commit & Push

```bash
git add .
git commit -m "feat: add speech tuning support"
git push origin feature/my-cool-feature
```

### 5. Open a Pull Request

* Target the `main` branch unless told otherwise.
* Add a clear PR description.
* Link related issues (e.g. `Fixes #12`).
* Add screenshots if it’s a UI change.

---

## 🧪 Areas You Can Contribute

| Area                | Description                                        |
| ------------------- | -------------------------------------------------- |
| 🗣️ Speech Accuracy | Improve STT transcription (Malayalam, noisy audio) |
| 🧠 NLP / LLM        | Custom prompts, reasoning logic, or memory support |
| 📞 VoIP Layer       | SIP handling, call state feedback, call logs       |
| 🔉 TTS Output       | Integrate new TTS libraries (Tortoise, Coqui)      |
| 📊 Dashboard UI     | Build a React-based call visualizer                |
| 📚 Docs             | Better setup guides, architecture, or tutorials    |
| 🐞 Bug Fixes        | Crash handling, edge cases, error logging          |

---

## 🤖 Code Style

* Python: Follow [PEP8](https://peps.python.org/pep-0008/)
* Use **async/await** for real-time tasks
* Avoid hardcoded paths, use `Pathlib`
* Avoid pushing `.env`, API keys, model files

---

## 🧠 Tips for First-Time Contributors

* Look for issues labeled `good first issue`
* Feel free to ask questions in Discussions
* Your idea doesn't have to be perfect — start small!

---

## 🙌 Code of Conduct

All contributors must adhere to our [Code of Conduct](https://github.com/Zentry/.github/blob/main/CODE_OF_CONDUCT.md). We foster a safe, welcoming space.

---

## 🧭 Need Help?

Create a new Discussion topic or open an issue. One of the maintainers will get back to you soon.

Happy hacking! 🚀
– **Team Zentry**
