# 🖋️ openCheck

**openCheck** is a premium, open-source, and entirely local-first writing assistant. It helps you improve your grammar, adjust your tone, and rewrite text without ever sending your data to the cloud.

## ✨ Key Features

- **Local-First & Offline**: Runs entirely on your machine using Llama-3.2-1B and LanguageTool.
- **Profile System**: Create multiple profiles to track your personal writing journey.
- **Smart Statistics**: Monitor your word count, correction rate, and activity over time.
- **7-Day Activity Chart**: Visualize your writing habits with a built-in sparkline dashboard.
- **Premium Dark UI**: A sleek, glassmorphism-inspired interface designed for focus.
- **Multiple Modes**:
    - **Grammar Fix**: Precise rule-based corrections.
    - **Formal/Casual Tone**: AI-powered stylistic adjustments.
    - **Rewrite**: Complete phrasing overhauls for better clarity.

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- macOS (Optimized for Metal/M-series chips)

### Installation & Launch
The easiest way to start openCheck is using the included launcher script:

1. Clone the repository:
   ```bash
   git clone https://github.com/pBariskan/grammarly-oss.git openCheck
   cd openCheck
   ```

2. Run the launcher:
   ```bash
   chmod +x start.sh
   ./start.sh
   ```

The script will automatically set up the environment, start the FastAPI server in the background, and open the application in your default browser at `http://localhost:8000`.

## 🛠️ Tech Stack

- **Backend**: FastAPI, Python, SQLite
- **AI/LLM**: llama-cpp-python (Llama-3.2-1B)
- **Grammar**: language-tool-python
- **Frontend**: Vanilla JavaScript, CSS (Modern Design Tokens), HTML5

## 🔒 Privacy
Your data never leaves your computer. openCheck is built for users who value privacy and want a powerful writing tool without the cloud subscription or tracking.

---
*Built with ❤️ by [pBariskan](https://github.com/pBariskan)*
