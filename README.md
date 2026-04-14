# 📝 Clinical Note Generator

AI-powered clinical note generation from patient encounters

![Python](https://img.shields.io/badge/Python-3.10+-blue) ![Ollama](https://img.shields.io/badge/Ollama-Local%20LLM-green) ![Gemma 3](https://img.shields.io/badge/Gemma%203-Google-orange) ![License](https://img.shields.io/badge/License-MIT-yellow) ![Privacy](https://img.shields.io/badge/Privacy-First-red)

## What It Does

- Generate structured clinical notes from patient encounter transcripts
- Extract vital signs, medications, and assessments automatically
- Format notes in standard medical terminology and structure
- Run entirely locally with Ollama and Gemma 3 for HIPAA compliance

## Tech Stack

- **Python 3.10+** — Core application logic
- **FastAPI** — High-performance API backend
- **Streamlit** — Interactive user interface
- **Ollama** — Local LLM runtime (ollama.com)
- **Gemma 3** — Google's open, efficient language model

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kennedyraju55/clinical-note-generator.git
   cd clinical-note-generator
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Pull the Gemma 3 model:**
   ```bash
   ollama pull gemma3:4b
   ```

4. **Run the application:**
   ```bash
   streamlit run app.py
   ```

## Architecture

```
User Interface (Streamlit)
         ↓
   FastAPI Backend
         ↓
   Ollama Runtime
         ↓
   Gemma 3 Model
         ↓
   Response Generation
```

## Why Local?

Clinical notes contain sensitive patient health information. By running Gemma 3 locally via Ollama, notes never leave your infrastructure, ensuring HIPAA compliance and data privacy.

### Key Privacy Benefits:

- **No External Calls** — All processing happens on your machine
- **No Data Transmission** — Sensitive information never leaves your infrastructure
- **Full Control** — You own and manage your data and model
- **Offline Capable** — Run completely disconnected from the internet

## Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (\git checkout -b feature/your-feature\)
3. Commit your changes (\git commit -m 'Add your feature'\)
4. Push to the branch (\git push origin feature/your-feature\)
5. Open a Pull Request

## License

MIT License — see [LICENSE](LICENSE) for details.

---

Part of [114+ privacy-first AI tools](https://github.com/kennedyraju55) by Nrk Raju