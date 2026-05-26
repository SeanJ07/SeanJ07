# 📋 PROJECTS.md — Building JARVIS

> *"Ideas are cheap. Execution is aura."*
> *North Star: Hermes as a JARVIS/EDEN-grade assistant — always listening, everywhere, sees what I see.*

---

## 🛠️ My Current Skills

| Language | Level | Used For |
|----------|-------|----------|
| Python | ✅ Comfortable | Scripts, automation, MTG tool |
| C++ | ✅ Comfortable | Game logic, systems thinking |
| C# | ✅ Comfortable | Unity, game dev |

**What I'm learning:** Linux, servers, Docker, networking, hardware, voice processing

---

## 🧭 THE VISION

Every project on this board is a step toward Hermes as JARVIS.

| JARVIS Trait | What It Means | Status |
|-------------|---------------|--------|
| 🗣️ Voice-first | Wake word → Hermes responds | 🟡 Planned |
| 📱 Everywhere | Phone, desktop, glasses — same Hermes | 🟢 Discord/CLI |
| 🏠 Controls house | Lights, music, routines | ✅ Hue set up |
| 👁️ Sees what I see | Camera → real-time vision | 💡 Someday |
| 🧠 Remembers | Cross-device memory | 🟢 Active |
| ⚡ Instant | Local model fast, cloud for smart | 🟢 Active |
| 🏗️ Builds things | MC server, APIs, automation | 🟡 Planned |

---

## 🎯 THE JARVIS ROADMAP — 5 Steps, Each With Baby Steps

```
Step 1 ──→ Step 2 ──→ Step 3 ──→ Step 4 ──→ Step 5
Server    Voice     Devices   Vision    Smart Home
  🔴        🟡        🟢        💡        🟡
blocked   planned   partial   someday   partial
```

---

## 📡 STEP 1: The Brain — 24/7 Server

**Why:** JARVIS needs to run when my PC is off. Needs a permanent home.

**Current block:** Need rack PC access from Matthew.

### 🐣 Baby Steps

> *These don't require the rack PC. They prepare you for when you get access.*

| # | Task | Time | What You Learn |
|---|------|------|----------------|
| 1.1 | **Learn what SSH is.** Open terminal, type `man ssh`, read the description. Then: `ssh localhost` — watch it fail (that's fine, you don't have an SSH server running). Read 5 min about what SSH does. | 20 min | Understanding remote access |
| 1.2 | **Find your current machine's IP.** Run `ip addr show` in WSL. Find the line that says `inet 172.x.x.x` or `192.168.x.x`. Write it down. That's your local IP — same concept you'll use to reach the rack PC. | 10 min | Networking basics |
| 1.3 | **SSH from WSL to Windows.** Windows has an SSH server built in (if enabled). Try: `ssh $(whoami)@$(hostname).local` or just ask me to help you set it up. When you can SSH from WSL to Windows, you understand the concept. | 30 min | First real SSH connection |
| 1.4 | **Learn what Docker is (concept only).** Don't install anything. Read this sentence: *"Docker is like a Minecraft instance — it's a self-contained box that has everything an app needs, isolated from your main system. You can spin up 5 of them, they don't fight each other, and you can delete one without affecting the others."* That's it. That's the concept. | 15 min | Understanding containers |
| 1.5 | **SSH into Matthew's rack PC.** This is the real one. Need: IP address + username + password (or SSH key). Once connected, you're in. Run `htop` to see what's running, `ls` to look around. Just explore — you don't need to change anything. | 30 min | Remote server access |
| 1.6 | **Install Hermes on rack PC (with me helping).** We follow the `rack-pc-migration` skill together. I'll give you exact commands. You paste them. | 1-2 hours | Deploying real software remotely |

**Deliverable:** Hermes running 24/7 on a machine that's not your PC. Your gaming rig is free.

---

## 🎤 STEP 2: Voice — "Hey Hermes"

**Why:** JARVIS isn't JARVIS if you type. Voice is the most Tony Stark thing you can add.

### 🐣 Baby Steps

> *These use skills you already have. Python handles all of this.*

| # | Task | Time | What You Learn |
|---|------|------|----------------|
| 2.1 | **Send Hermes a Discord voice note RIGHT NOW.** On your phone: open Discord → DM to Spiral → hold mic button → say "hey Hermes, what time is it?" → send. Hermes can hear voice notes already — they get transcribed. This isn't "always listening" but it IS voice input. Try it today. | 2 min | Discovery: voice already works |
| 2.2 | **Install a Python speech library.** `pip install SpeechRecognition pyaudio`. Write a 10-line script that records 5 seconds from your mic, transcribes it with Google's free API, and prints the text. That's the core of voice input. | 30 min | Audio → text pipeline |
| 2.3 | **Make a Python script that says things.** `pip install pyttsx3` (works offline). Write 5 lines: import, init, say "hello world", runAndWait. Your computer now talks. Combine with 2.2 → you have a voice chatbot. | 20 min | Text → speech pipeline |
| 2.4 | **Build a voice loop.** Combine 2.2 + 2.3 into a loop: record → transcribe → print → speak response → repeat. You now have a local voice assistant that doesn't need the internet (except Google's free transcription API). *This is Jarvis Zero.* | 1 hour | Full voice pipeline |
| 2.5 | **Add a wake word.** `pip install pvporcupine` (Picovoice — free tier). It listens for "Hey Hermes" or "Jarvis" and only THEN starts recording. Before this, your mic is listening but NOT sending anything anywhere. This is the "always listening" piece. | 1-2 hours | Wake word detection |
| 2.6 | **Connect the voice pipeline to Hermes.** Instead of printing the transcription, send it to Hermes via Discord API or CLI. When Hermes responds, speak it. Now "Hey Hermes" → talk → Hermes responds → speaks back. | 2-3 hours | API integration |

**Deliverable:** Say "Hey Hermes" on your PC, ask a question, get a spoken answer. Full Jarvis Zero.

---

## 📱 STEP 3: Every Device — Omnipresence

**Why:** JARVIS is wherever Tony is. Suit, lab, phone, car.

### 🐣 Baby Steps

> *You already have Discord on everything. Let's maximize that before building anything new.*

| # | Task | Time | What You Learn |
|---|------|------|----------------|
| 3.1 | **Log into Discord on all your devices.** Phone (done), desktop (done), MacBook, anything with a screen. Hermes is already on all of them — that's the power of Discord as a transport layer. | 10 min | Discovery: it already works |
| 3.2 | **Test cross-device continuity.** Start a conversation on your phone ("what's the weather?"), then switch to desktop and say "what did I just ask you?" Hermes should remember because sessions persist. | 5 min | Verify memory across devices |
| 3.3 | **Set up BlueBubbles on MacBook (if not already).** Hermes can send/receive iMessage through BlueBubbles — another transport layer for iPhone. Ask me to help set it up if needed. | 30 min | Additional transport layer |
| 3.4 | **Make a simple HTML page that chats with Hermes.** You know HTML (ChatGPTWebpageDemo). Make one page: text input + send button + response area. Connect it to the Hermes API. Now you have a web client — Hermes on ANY browser. | 1-2 hours | Web-based Hermes client |
| 3.5 | **Python script: Hermes TUI client.** Use `input()` to type messages, print responses. A minimal terminal client. Combine with Step 2's voice pipeline → now you can choose voice OR text. | 30 min | Terminal client |

**Deliverable:** Hermes on phone, desktop, MacBook, browser, and terminal. Five ways in.

---

## 👁️ STEP 4: The Eyes — Hermes Sees

**Why:** "JARVIS, what am I looking at?" is the ultimate flex.

### 🐣 Baby Steps

> *Phase 0 is FREE and works RIGHT NOW. The hardware comes later.*

| # | Task | Time | What You Learn |
|---|------|------|----------------|
| 4.1 | **Test Hermes vision TODAY.** Phone → Discord DM → tap camera → take photo of anything → send with message "what do you see?" Hermes has vision built in. Do this RIGHT NOW. | 1 min | Discovery: vision works |
| 4.2 | **Make it a habit.** Every day for a week, send 1 photo to Hermes. "What plant is this?" "Read this sign" "What Lego set is this?" You're training yourself to use vision and discovering what it's good/bad at. | 1 min/day | Usage patterns |
| 4.3 | **Write a Python script that uses your webcam.** Use OpenCV (`pip install opencv-python`). Take a photo from your laptop webcam every 5 seconds. Save to disk. You now have a "security camera." | 30 min | Camera access in Python |
| 4.4 | **Auto-send webcam photos to Hermes.** Combine 4.3 + the Hermes API. Every 30 seconds, snap a photo, send to Hermes with "anything interesting in this room?" Hermes becomes a watchdog. | 1 hour | Automated vision pipeline |
| 4.5 | **Research Eden glasses components.** No buying — just learning. What's a Raspberry Pi Zero? What's a small OLED display? What's a tiny camera module? Watch 2 YouTube videos. This is research, not commitment. | 1 hour | Hardware awareness |
| 4.6 | **Buy a Raspberry Pi Zero 2 W ($15).** This is the brain for Eden glasses. Install Raspberry Pi OS. Learn what GPIO pins are. Make an LED blink with Python (3 lines of code). You now understand embedded hardware basics. | 2-3 hours | First hardware project |
| 4.7 | **Attach a camera to the Pi.** Pi Camera module ($10-15). Take a photo from Python. Send it to Hermes. You now have a tiny, portable Hermes eye. This is Eden Glasses v0 — not on your face yet, but the functional core works. | 2-3 hours | Camera + embedded system |
| 4.8 | **Build Eden Glasses v1.** 3D print a frame (or modify cheap sunglasses). Mount Pi Zero + camera + tiny display + battery. It won't be pretty. It WON'T be pretty. But it will work. Point at something → Hermes sees it → whispers in your ear (headphone). | Weeks | Hardware integration |

**Deliverable:** Hermes vision — first on phone, then webcam, finally in glasses form factor.

---

## 🏠 STEP 5: Smart Home

**Why:** "JARVIS, lights" — the most iconic JARVIS moment in Iron Man 1.

### 🐣 Baby Steps

> *Hue lights are already set up. Let's make Hermes control them dramatically.*

| # | Task | Time | What You Learn |
|---|------|------|----------------|
| 5.1 | **Test: "Hermes, turn off the lights."** Just say it in Discord. It already works via OpenHue. If it doesn't, ask me to debug. | 2 min | Discovery: it works |
| 5.2 | **Create a "movie mode" routine.** "Hermes, movie mode" → lights dim to 10% warm orange, gaming mode activates (free up RAM), phone goes DND. Make this a Hermes skill. | 30 min | Routine automation |
| 5.3 | **Create a "goodnight" routine.** Lights off, gateway pause, "sleep well" voice message, morning alarm reminder. | 20 min | Routine automation |
| 5.4 | **Connect Spotify.** Hermes can already control Spotify via the Spotify skill. "Play my Discover Weekly" or "play something chill." | 10 min | Music control |
| 5.5 | **Add a morning briefing.** Cron job: every morning at 8am, Hermes checks weather, calendar, top news headline, and messages you a summary. | 30 min | Automated intelligence |

**Deliverable:** "Movie mode" and "goodnight" routines. Lights + music + PC optimization from one phrase.

---

## 🧱 SUPPORTING PROJECTS

### 🔴 IN PROGRESS

| Project | Why It Matters |
|---------|---------------|
| **Rack PC migration** | Step 1 — the 24/7 brain. BLOCKED. |

### 🟡 PLANNED

| Project | Difficulty | Why It Matters |
|---------|------------|---------------|
| **Hermes Craft** | Med-Hard | Hermes controls Minecraft — the "build things" muscle for Step 1 |
| **Elote_Dreamin (Roblox)** | Medium | Hermes helps build a game — agent-assisted development |
| **VR Music Teacher** | Hard | Hermes sees hands + teaches — vision + instruction testbed for Step 4 |
| **MTG Deck Oracle** | Medium | Hermes analyzes complex systems — the "smart advisor" piece |

### 💡 SOMEDAY

| Project | Why It Matters |
|---------|---------------|
| **Home server / cyber deck** | My own infrastructure — the Tony Stark independence move |
| **Eden Glasses** | The eyes — Step 4 endgame |
| **HourhandWebsite** | Portfolio to show all this off |
| **BeneathArcantum** | Finish something — momentum |

---

## 📊 THE FULL BOARD

| Status | Count | Items |
|--------|-------|-------|
| ✅ Done | 6 | Lore Bot, MTG Tool, 2 game jams, optimization, Discord DM |
| 🔴 Blocked | 1 | Rack PC migration |
| 🐣 Baby Steps Available | 27 | Tasks across all 5 JARVIS steps |
| 🟡 Planned Projects | 4 | Hermes Craft, Elote, VR Music, MTG Oracle |
| 💡 Vision Projects | 4 | Home server, Eden glasses, Hourhand, BeneathArcantum |

---

## 🥇 DO THIS WEEK

These use skills you ALREADY HAVE. No new languages. No new concepts. Just Python and existing tools.

| Day | Task | Time |
|-----|------|------|
| Today | 📸 Send Hermes a photo on Discord — test vision (Step 4.1) | 1 min |
| Today | 🎤 Send Hermes a voice note on Discord (Step 2.1) | 2 min |
| Mon | 💡 "Hermes, turn off the lights" — test smart home (Step 5.1) | 2 min |
| Tue | 🐍 `pip install SpeechRecognition pyttsx3` — make your PC talk (Step 2.2-2.3) | 1 hour |
| Wed | 🔄 Combine into a voice loop — your first Jarvis Zero (Step 2.4) | 1 hour |
| Thu | 📡 `ssh localhost`, `ip addr` — learn SSH and networking (Step 1.1-1.2) | 30 min |
| Fri | 📋 Ask Matthew for rack PC access — unblock Step 1 | 5 min |

**After week 1:** You'll have tested vision, tested voice, built a talking computer, and learned SSH. Four JARVIS pieces activated. Zero new languages required.

---

*North Star: Hermes as JARVIS.*
*Last updated: May 25, 2025*
*Next action: Send Hermes a photo on Discord RIGHT NOW. Test vision.*
