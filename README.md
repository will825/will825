## Hi, I'm Will

I'm an audio engineer who became a software engineer, and I build production tools for music and audio — the kind of thing I always wished existed when I was behind the console.

For years my job was listening closely: editing dialogue for award-winning films, mixing live rooms, and running Terra Echo Studios, my own audio practice. The more I worked, the more I ran into the same gaps — tools that were slow, locked behind subscriptions, or just didn't exist. So I taught myself to build them. These days I work where audio craft meets software: writing Rust, serving ML models on-device, wiring up LLMs, and shipping full-stack apps end to end. I care about how things sound, how code reads, and whether the thing actually works for the person using it.

I'm looking for a role where I can do this full-time, ideally somewhere at the intersection of audio, AI, and music technology.

---

## Things I've built

### Plumb — offline audio analyzer for masters

*Live and shipping.* A native Mac app that gives mastering engineers a fast, accurate readout on a finished mix — true peak, integrated/short-term/momentary loudness, loudness range, PLR, PSR, clipping, and DC offset — then checks it against real delivery specs (Spotify, Apple Music, EBU R128, Netflix, and more) so you know before you upload whether a platform is going to turn it down. The interesting part is the measurement layer: loudness and true-peak math built on libebur128 so the standards-critical parts are correct, not hand-rolled, feeding a modular dashboard — spectrogram, spectrum, goniometer, tonal balance against a reference track — plus one-click PDF/CSV reports for clients. Shipped solo as a signed universal binary.

Rust · Tauri 2 · React · TypeScript · libebur128 — [Download](https://terraecho.gumroad.com/l/plumb) · [Repo](https://github.com/will825/plumb)

### Fissure — AI stem splitter for macOS

*Live and shipping.* A native Mac app that splits any song into clean stems — vocals, drums, bass, and more — running entirely offline. The interesting part is under the hood: a Rust core (Tauri 2) that serves three ONNX audio-ML models through an audio pipeline I wrote by hand — decode, resample, STFT/ISTFT, overlapping-chunk inference, 24-bit WAV out — behind a lazy session pool with CoreML-or-CPU execution-provider fallback. Built solo, end to end, and shipped as a signed universal binary.

Rust · Tauri 2 · ONNX Runtime · React · TypeScript — [Download](https://terraecho.gumroad.com/l/rlpqdr) · [Repo](https://github.com/will825/FISSURE)

### Resonance — AI chord progression generator

*Live.* Describe a vibe in plain language and get a musically-correct, voice-led chord progression you can hear in the browser and export as MIDI. The interesting part is the architecture: a Groq LLM supplies only the creative intent (chords as Roman numerals), and a deterministic TypeScript theory engine renders guaranteed-correct notes — so the output is always valid, and it degrades gracefully to a curated fallback when the AI is offline.

Next.js · TypeScript · Groq · Tone.js · @tonejs/midi — [Live](https://resonance-beige-omega.vercel.app) · [Repo](https://github.com/will825/resonance)

### SkyForge — space-intelligence dashboard

A full-stack dashboard that pulls 10+ live feeds (NASA, NOAA, ISS telemetry) into one place, with async caching, Pydantic v2 schema validation, a real pytest suite, and one-command Docker Compose + nginx deployment.

Python · FastAPI · React · TypeScript · Docker — [Repo](https://github.com/will825/skyforge)

### Terra Echo Studios — studio site

The site for my audio studio, designed and built from scratch: a React 18 + Vite single-page app (React Router, Tailwind, Keystatic CMS) with scroll-reveal animations and ambient audio, deployed on Netlify.

React · Vite · Tailwind · Keystatic — [Live](https://terraechostudio.com) · [Repo](https://github.com/will825/terra-echo-website-2.0)

### Job Hunter — multi-source job pipeline

A Python tool that polls 80+ company ATS APIs (Greenhouse, Lever, Ashby) and RSS feeds, scores each listing against a weighted keyword model, deduplicates in SQLite, and pushes ranked Discord alerts on a schedule.

Python · Playwright · httpx · SQLite — [Repo](https://github.com/will825/job-hunter)

### More

The earlier prototype I focused down into Fissure — a [Music Production Intelligence Suite](https://github.com/will825/terra-echo-labs-music-assistant) (Electron, React, FastAPI, Demucs v4) with an LLM chord-progression generator, MIDI engine, and stem splitter — plus a handful of Linux/Raspberry Pi systems builds: real-time monitoring as a systemd service, journald log-alerting with regex detection, and an IoT sensor platform with data-validation logic.

---

## What's next

Fissure is the first release in a line of native, offline-first audio tools I'm building for producers — creative effects, mastering utilities, and audio-ML apps, each aimed at a specific gap I've hit in my own work. A few on the bench:

- **Blueprint** — an AI mastering-chain builder: analyze a track against a reference, then recommend a signal chain from the user's own plugins (Rust audio analysis with LLM interpretation).
- **Fragment** — a real-time granular texture engine with macro-driven controls, built for atmospheric and electronic music.
- **Cone** — a dual-input low-end phase-coherence tool for the classic kick-versus-bass problem.

Same idea as Fissure every time: native, offline, no subscriptions, built for how people actually work.

---

## What I work with

- **Languages** — Rust, TypeScript, Python, JavaScript, SQL
- **AI / ML** — ONNX Runtime (on-device serving), htdemucs, MDX-Net, Demucs/PyTorch, Claude / OpenAI / Groq APIs, agentic dev (Claude Code, Cursor)
- **Backend** — Tauri 2 (Rust), FastAPI, REST, Pydantic v2, SQLite, Docker, pytest
- **Frontend** — React, Vite, TypeScript, Tailwind, Electron, Chart.js

---

## A little more

I studied Audio Engineering Technology at Belmont University (minor in Music Business), and I'm based in Boone, North Carolina, where I run Terra Echo Studios — audio production and the software behind it. Mostly I just like making things and creating!

**Reach me:** terraechostudios@gmail.com · · [terraechostudio.com](https://terraechostudio.com)
