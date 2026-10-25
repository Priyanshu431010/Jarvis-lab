# 🤖 J.A.R.V.I.S. — Hacker-Style AI Assistant

A Tony Stark-inspired desktop assistant with a hacker terminal interface, an animated AI character, voice commands and live system monitoring.
Built with **Python + Java + HTML + CSS + JavaScript**.

## ✨ Features
- 🎭 Animated AI character (blinking eyes that follow your mouse, talking mouth)
- 🟢 Matrix-rain hacker UI with glitch title, neon panels and 3 themes (green / red / blue)
- 🎤 Voice commands (Chrome) + text-to-speech replies
- 🖥 Live CPU / RAM / Disk / Battery monitor with graph
- ☕ Java module that reports OS, cores, memory and load
- 🧰 Tools: calculator, password generator, SHA-256 hash, Base64, localhost port scanner, network info
- 🚀 Launch websites & apps by command (YouTube, Google, GitHub, Gmail, Notepad, Calculator...)
- ☑ Missions (to-do) and timers
- 🧠 Optional **Holo Lab** — hand-gesture 3D holograms using your webcam

## 🚀 Quick Start
```bash
git clone https://github.com/<your-username>/jarvis.git
cd jarvis
pip install psutil      # optional (for CPU/RAM stats)
python server.py
```
The browser opens automatically at `http://127.0.0.1:8765`.

**Requirements:** Python 3.8+, Chrome (for voice), Java 11+ (optional, for the Java panel).

## 💬 Example commands
| Command | What it does |
|---|---|
| `open youtube` | Opens YouTube |
| `play arijit singh` | Searches YouTube |
| `calc 25*4+10` | Calculator |
| `password 20` | 20-char secure password |
| `scan` | Scans common ports on your own PC |
| `todo add finish project` | Adds a mission |
| `timer 5 min` | Sets a timer |
| `hack` | Red-alert mode |
| `help` | All commands |

## 📁 Structure
```
server.py        # Python backend (localhost only)
SystemInfo.java  # Java system-info module
index.html       # Interface
style.css        # Hacker theme + character animation
app.js           # Commands, voice, live stats
jarvis_holo_lab.html  # Webcam hand-gesture holograms (MediaPipe + Three.js)
```

## 🔒 Security
The server binds to `127.0.0.1` only. Only whitelisted apps/sites can be opened, the calculator uses a safe AST evaluator, and the port scanner targets localhost only.

## 📜 License
MIT
