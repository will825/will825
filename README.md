Hi, I'm Will

I'm an audio engineer who became a software engineer, and I build production tools for music and audio — the kind of thing I always wished existed when I was behind the console.

For six years my job was listening closely: editing dialogue for award-winning films, mixing live rooms, and running Terra Echo Studios, my own audio practice. The more I worked, the more I ran into the same gaps — tools that were slow, locked behind subscriptions, or just didn't exist. So I taught myself to build them. These days I work where audio craft meets software: writing Rust, serving ML models on-device, wiring up LLMs, and shipping full-stack apps end to end. I care about how things sound, how code reads, and whether the thing actually works for the person using it.

I'm looking for a role where I can do this full-time, ideally somewhere at the intersection of audio, AI, and music technology.


Things I've built

Fissure — AI stem splitter for macOS

Live and shipped. A native Mac app that splits any song into clean stems — vocals, drums, bass, and more — running entirely offline. The interesting part is under the hood: a Rust core (Tauri 2) that serves three ONNX audio-ML models through an audio pipeline I wrote by hand — decode, resample, STFT/ISTFT, overlapping-chunk inference, 24-bit WAV out — behind a lazy session pool with CoreML-or-CPU execution-provider fallback. Built solo, end to end, and shipped as a signed universal binary.

Rust · Tauri 2 · ONNX Runtime · React · TypeScript  —  Download · Repo

SkyForge — space-intelligence dashboard

A full-stack dashboard that pulls 10+ live feeds (NASA, NOAA, ISS telemetry) into one place, with async caching, Pydantic v2 schema validation, a real pytest suite, and one-command Docker Compose + nginx deployment.

Python · FastAPI · React · TypeScript · Docker  —  Repo

Music Production Intelligence Suite

The earlier desktop app I eventually narrowed down into Fissure: an LLM chord-progression generator (Groq / Llama 3.3 70B), a MIDI engine, a stem splitter, and a music-theory reference. A good lesson in cutting scope to ship something sharp.

Electron · React · FastAPI · Demucs v4  —  Repo

Systems and IoT

Smaller, practical builds: a real-time Linux monitor running as a systemd service on a Raspberry Pi, a journald log-alerting service with regex pattern detection and structured JSON output, and an IoT sensor platform with data-validation logic baked in.


What's next

Fissure is the first release in a line of native, offline-first audio tools I'm building for producers — creative effects, mastering utilities, and audio-ML apps, each aimed at a specific gap I've hit in my own work. A few on the bench:


Blueprint — an AI mastering-chain builder: analyze a track against a reference, then recommend a signal chain from the user's own plugins (Rust audio analysis with LLM interpretation).
Fragment — Granular texture engine — real-time granular processor with macro-driven controls designed for atmospheric/electronic music.
Cone — a dual-input low-end phase-coherence tool for the classic kick-versus-bass problem.


Same idea as Fissure every time: native, offline, no subscriptions, built for how people actually work.


What I work with

Languages - Rust, TypeScript, Python, JavaScript, SQL
AI -  / MLONNX Runtime (on-device serving), htdemucs, MDX-Net, Demucs/PyTorch, Claude / OpenAI / Groq APIs, agentic dev (Claude Code, Cursor, Codex)
Backend - Tauri 2 (Rust), FastAPI, REST, Pydantic v2, SQLite, Docker, pytest
Frontend - React, Vite, TypeScript, Tailwind, Electron, Chart.js
Audio - Pro Tools, Logic Pro, iZotope RX, STFT/ISTFT, mastering, Dante (Level 3)SystemsLinux, systemd, Raspberry Pi, universal binaries, Git


A little more

I studied Audio Engineering Technology at Belmont University (minor in Music Business), and I'm based in Boone, North Carolina, where I run Terra Echo Studios — audio production and software. Mostly I just like building and creating!

Reach me: Terraechostudios@gmail.com· terraechostudio.com
