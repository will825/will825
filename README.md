Hi, I'm Will 👋

Audio engineer turned software builder — I ship production-grade tools for music and audio.

I spent six years developing a professional ear: editing dialogue for award-winning films, mixing live shows, and running Terra Echo Studios, my independent audio studio. Somewhere along the way I started building the tools I wished existed. Now I work at the intersection of audio craft and software — serving audio-ML models on-device, integrating LLMs into real workflows, and shipping full-stack apps end to end.


🚀 What I'm building

Fissure — AI Stem Splitter for Mac  ·  live & shipping
A native macOS app that separates any song into clean stems — vocals, drums, bass, and more — running 100% offline. A Rust core (Tauri 2) serves three ONNX audio-ML models (htdemucs 4-/6-stem + MDX-Net vocal isolation) over a hand-built audio pipeline (decode → resample → STFT/ISTFT → inference → 24-bit WAV), with a lazy ONNX session pool and CoreML/CPU execution-provider fallback. Shipped as a signed universal binary.
Rust · Tauri 2 · ONNX Runtime · React · TypeScript
▶ Download on Gumroad · Repo

SkyForge — Full-stack space-intelligence dashboard integrating 10+ live APIs (NASA, NOAA, ISS telemetry) with async caching, Pydantic v2 schema validation, a pytest suite, and one-command Docker Compose + nginx deployment.
Python · FastAPI · React · TypeScript · Docker

Music Production Intelligence Suite — Earlier macOS desktop app: LLM chord-progression generator (Groq / Llama 3.3 70B), MIDI engine, stem splitter, and music-theory reference. The broad prototype I focused down into Fissure.
Electron · React · FastAPI · Demucs v4

Systems & IoT — SysMon Dashboard (real-time Linux monitoring as a systemd service on a Pi), Log Alert Service (journald + regex pattern detection, structured JSON alerts), and Mushroom Monitor (IoT sensor platform with data-validation logic).


🧰 What I work with

Languages   Rust · TypeScript · Python · JavaScript · SQL
AI / ML     ONNX Runtime (on-device serving) · htdemucs · MDX-Net · Demucs/PyTorch · Claude / OpenAI / Groq APIs / Cursor
Backend     Tauri 2 (Rust) · FastAPI · REST · Pydantic v2 · SQLite · Docker · pytest
Frontend    React · Vite · TypeScript · Tailwind · Electron · Chart.js
Audio       Pro Tools · Logic Pro · iZotope RX · STFT/ISTFT · Dante 
Systems     Linux · systemd · Raspberry Pi · universal binaries · Git


🌲 A bit more


🎓 B.S. Audio Engineering Technology — Belmont University (Minor: Music Business)
🏔️ Based in Boone, NC
🎙️ Founder of Terra Echo Studios — audio production & software 
🔧 I like building things 


Currently building at the intersection of audio, AI, and music technology — and shipping it.

📬 terraechostudios@gmail.com · LinkedIn · terraechostudio.com
