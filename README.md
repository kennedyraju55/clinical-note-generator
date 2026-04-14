# 📝 Clinical Note Generator

Generate structured clinical notes from patient interactions using privacy-first AI.

[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![Ollama](https://img.shields.io/badge/Ollama-Local%20AI-ff6b6b?logo=ollama)](https://ollama.com)
[![Gemma 3](https://img.shields.io/badge/Gemma%203-Powered-orange?logo=google)](https://ai.google.dev/gemma)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Privacy First](https://img.shields.io/badge/Privacy-First-purple)](README.md)

## What It Does

- Transforms unstructured patient interaction data into HIPAA-compliant structured clinical notes
- Supports multiple clinical note formats (SOAP, PROGRESS, CONSULTATION)
- Automatically extracts key clinical entities (diagnoses, medications, procedures)
- Runs entirely on your machine - no cloud APIs, no patient data sent anywhere

## Tech Stack

- **LLM**: Gemma 3 (via Ollama)
- **Backend**: FastAPI
- **Frontend**: Streamlit
- **Language**: Python 3.9+
- **Architecture**: 100% Local, Privacy-First

## Quick Start

### Prerequisites
- Python 3.9 or higher
- [Ollama](https://ollama.com) installed and running
- 8GB+ RAM recommended
- GPU optional but recommended for faster inference

### Installation Steps

1. **Clone the repository**
   `ash
   git clone https://github.com/kennedyraju55/clinical-note-generator.git
   cd clinical-note-generator
   `

2. **Install dependencies**
   `ash
   pip install -r requirements.txt
   `

3. **Start Ollama** (in a separate terminal)
   `ash
   ollama run gemma3
   `

4. **Run the application**
   `ash
   streamlit run app.py
   `

The application will be available at http://localhost:8501

## Architecture

\\\
User Input
    ↓
  Streamlit UI
    ↓
  FastAPI Backend
    ↓
  Ollama + Gemma 3
    ↓
  Local Response (No Cloud)
\\\

Everything runs locally on your machine. No external API calls. No data leaves your device.

## Why Local?

Healthcare data is among the most sensitive information. Clinical notes contain PHI (Protected Health Information) that's strictly regulated under HIPAA. By running locally with Ollama and Gemma 3, you maintain 100% control over patient data - it never leaves your facility, never touches external servers, and complies with data residency requirements.

**Key Benefits:**
- ✅ **Compliant**: Meets HIPAA, GDPR, and institutional privacy requirements
- ✅ **Offline**: Works without internet connection
- ✅ **Fast**: No network latency, instant local inference
- ✅ **Secure**: Healthcare data never leaves your control
- ✅ **Custom**: Fine-tune models on your institution's data

## Configuration

See config.py for customizable settings:
- Model parameters
- Batch processing options
- Output formats
- Privacy settings

## Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch (\git checkout -b feature/amazing-feature\)
3. Commit your changes (\git commit -m 'Add amazing feature'\)
4. Push to the branch (\git push origin feature/amazing-feature\)
5. Open a Pull Request

## License

MIT License - see [LICENSE](LICENSE) for details

---

**Part of 114+ privacy-first AI tools by Nrk Raju**