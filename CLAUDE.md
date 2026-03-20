# Project Overview
`grammarly-oss` is a local, offline, open-source grammar and style improvement tool.

## Architecture
The system architecture has two layers:
1. **MANUAL LAYER** (build first): User pastes text into a local web UI, clicks "Improve", Phi-3 Mini model returns multiple suggestions (grammar fix, formal tone, casual tone, rewrite). FastAPI server on localhost:8000.
2. **AUTO LAYER** (build later): Real-time grammar checking while typing in any webpage, using a lightweight FLAN-T5-Large model.

## Tech Stack
- **Language Models**: Phi-3 Mini (via HuggingFace Transformers, 4-bit quantized), FLAN-T5-Large (later)
- **Backend API**: Python 3.11+, FastAPI, Uvicorn (localhost:8000)
- **Frontend**: Plain HTML/CSS/JS (no frameworks)
- **Extensions**: Chrome Extension MV3 (later), macOS Swift layer (later)

## Component Connections
- UI → `POST /improve` → FastAPI → Phi-3 Mini → returns 4 suggestions
- The `/improve` endpoint accepts: `{"text": "...", "mode": "grammar"|"formal"|"casual"|"rewrite"}`

## Coding Conventions
- **Python**: Use `black` syntax formatting and type hints.
- **JavaScript**: Use ES modules, no frameworks.

## How to Run Locally
*(To be detailed as implementation progresses)*
