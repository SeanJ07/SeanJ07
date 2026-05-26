# 📋 PROJECTS.md — Building JARVIS

> *"Ideas are cheap. Execution is aura."*
> *North Star: Hermes as JARVIS/EDEN — always listening, everywhere, sees what I see.*

---

## 🛠️ My Current Skills

| Language | Level | Used For |
|----------|-------|----------|
| Python | ✅ Comfortable | Scripts, automation, MTG tool |
| C++ | ✅ Comfortable | Game logic, systems thinking |
| C# | ✅ Comfortable | Unity, game dev |

**Learning:** Linux, servers, Docker, networking, hardware, voice processing

---

## 🧭 THE VISION

| JARVIS Trait | Status |
|-------------|--------|
| 🗣️ Voice-first | 🟡 Planned |
| 📱 Everywhere | 🟢 Discord/CLI |
| 🏠 Smart home | ✅ Hue active |
| 👁️ Vision | 💡 Someday |
| 🧠 Memory | 🟢 Active |
| ⚡ Instant | 🟢 Active |
| 🏗️ Builds things | 🟡 Planned |

---

## 🔴 IMMEDIATE ACTIONS (highest priority, minutes each)

These unblock everything else. Do them right now.

| # | Action | Time | Unlocks |
|---|--------|------|---------|
| 1 | 🔗 **Ask Matthew to add Spiral to shared Discord server** — unblocks Hermes ↔ Ares collab | 2 min | Inter-agent communication, Jenkins Robotics collab |
| 2 | 🖥️ **Ask Matthew for rack PC access** — unblocks Step 1 (24/7 server) | 1 min | JARVIS server, Hermes Craft, Docker migration |
| 3 | 🔑 **Add SSH key to GitHub** — paste clipboard key at github.com/settings/ssh/new | 1 min | Clean git pushes, no more token workarounds |
| 4 | 📸 **Test Hermes vision** — Discord DM → send photo → "what do you see?" | 1 min | Vision pipeline proof-of-concept |
| 5 | 🎤 **Test Hermes voice** — Discord DM → hold mic → send voice note | 2 min | Voice pipeline proof-of-concept |

**Total: 7 minutes. Unlocks 4 major threads.**

---

## 🎯 THE JARVIS ROADMAP

```
Step 1 ──→ Step 2 ──→ Step 3 ──→ Step 4 ──→ Step 5
Server    Voice     Devices   Vision    Smart Home
  🔴        🟡        🟢        💡        🟡
```

---

## 📡 STEP 1: 24/7 Server

**Blocked by:** Need rack PC access from Matthew.

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 1.1 | Learn SSH: `man ssh`, try `ssh localhost` | 20 min |
| 1.2 | Find your local IP: `ip addr show` | 10 min |
| 1.3 | SSH from WSL to Windows | 30 min |
| 1.4 | Learn Docker concept (no install needed) | 15 min |
| 1.5 | SSH into Matthew's rack PC — explore | 30 min |
| 1.6 | Install Hermes on rack PC (with my help) | 1-2 hours |

---

## 🎤 STEP 2: Voice — "Hey Hermes"

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 2.1 | Send voice note on Discord (works NOW) | 2 min |
| 2.2 | `pip install SpeechRecognition pyaudio` — record + transcribe | 30 min |
| 2.3 | `pip install pyttsx3` — make PC talk | 20 min |
| 2.4 | Build voice loop (record → transcribe → speak → repeat) | 1 hour |
| 2.5 | Add wake word: `pip install pvporcupine` | 1-2 hours |
| 2.6 | Connect voice pipeline to Hermes | 2-3 hours |

---

## 📱 STEP 3: Every Device

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 3.1 | Log into Discord on all devices | 10 min |
| 3.2 | Test cross-device memory continuity | 5 min |
| 3.3 | Set up BlueBubbles on MacBook | 30 min |
| 3.4 | Build web-based Hermes chat client | 1-2 hours |
| 3.5 | Python TUI client for terminal | 30 min |

---

## 👁️ STEP 4: Vision / Eden Glasses

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 4.1 | Send photo on Discord — test vision (works NOW) | 1 min |
| 4.2 | Daily photo habit for 1 week | 1 min/day |
| 4.3 | Python webcam capture with OpenCV | 30 min |
| 4.4 | Auto-send webcam photos to Hermes | 1 hour |
| 4.5 | Research Eden glasses components | 1 hour |
| 4.6 | Buy Raspberry Pi Zero 2 W ($15) | 2-3 hours |
| 4.7 | Attach camera to Pi, send photos to Hermes | 2-3 hours |
| 4.8 | Build Eden Glasses v1 (3D print frame + mount) | Weeks |

---

## 🏠 STEP 5: Smart Home

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 5.1 | Test: "Hermes, turn off the lights" (works NOW) | 2 min |
| 5.2 | Create "movie mode" routine | 30 min |
| 5.3 | Create "goodnight" routine | 20 min |
| 5.4 | Connect Spotify control | 10 min |
| 5.5 | Morning briefing cron job | 30 min |

---

## 🔗 STEP 6: HERMES ↔ ARES — INTER-AGENT COMMUNICATION 🆕

**Why:** Matthew's agent Ares runs on his Mac Studio, connects to the rack PC, and is building Jenkins Robotics. Two brothers, two agents, one mission.

**Current state:** Matthew needs to invite Spiral to the shared Discord server. Both agents are Discord-native.

### 🐣 Baby Steps

| # | Task | Time | Who |
|---|------|------|-----|
| 6.1 | Matthew invites Spiral (bot ID: 1507507057457581191) to shared server | 5 min | Matthew |
| 6.2 | Hermes pings Ares in shared channel: "Testing inter-agent comms" | 2 min | Sean + Hermes |
| 6.3 | Hermes asks Ares for robotics status update | 5 min | Sean + Hermes |
| 6.4 | Create `jenkins-robotics` shared GitHub repo | 15 min | Sean + Matthew |
| 6.5 | Both agents given repo access — collaborative workspace | 5 min | Matthew |
| 6.6 | First collab: Hermes writes YT script, Ares provides technical specs | 1 hour | Both agents |
| 6.7 | Cron sync loop: Hermes checks scout-system daily for updates | 30 min | Hermes |

**Deliverable:** Two AI agents collaborating across GitHub + Discord. Sean runs creative/YouTube. Matthew runs engineering/robotics. Agents coordinate automatically.

**Related shared spaces:**
- `shuwalker/scout-system` — campus job + scholarship pipeline (already shared)
- `shuwalker/ARES` — Matthew's embodied AI OS (Swift, macOS daemon, face/voice/sensors)
- Hermes → Ares → Jenkins Robotics YouTube content pipeline

---

## 🎥 JENKINS DIGITAL DESIGN — STEAM YouTube 🆕

**Why:** Revival of Hourhand Studios. Each contributor teaches their passion.

| Lane | Contributor | Content |
|------|------------|---------|
| 🎵 Music & Sound | [TBD] | Production, sound design, audio engineering |
| 💻 Computer Engineering | [TBD] | Hardware, systems, embedded programming |
| 🔭 Astronomy | [TBD] | Space, telescopes, astrophotography |
| 🎨 Digital Art | [TBD] | Illustration, design, creative tools |
| 🔒 Cybersecurity | [TBD] | Ethical hacking, network defense, CTFs |
| 🤖 Jenkins Robotics | Matthew + Ares | Robot builds, behind-the-scenes, tech specs |

**Sean's role:** Producer, editor, brand manager. Hermes = content assistant.

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 7.1 | Create YouTube channel + banner + about section | 1 hour |
| 7.2 | Design JDD logo/branding | 2 hours |
| 7.3 | Confirm contributor lineup — who's in? | Varies |
| 7.4 | Plan first 5 video topics | 1 hour |
| 7.5 | Hermes helps write first video script | 1 hour |
| 7.6 | Set up Hermes cron for content calendar management | 30 min |
| 7.7 | Record + edit + publish first video | Varies |
| 7.8 | Build Jenkins Robotics YT segment (collab with Matthew) | Ongoing |

---

## 🏥 JENKINS HEALTH INSURANCE AGENT — Next Steps 🆕

**Repo:** [ChatGPTWebpageDemo](https://github.com/SeanJ07/ChatGPTWebpageDemo)
**Status:** Chat UI done. Backend connection needed.

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 8.1 | Connect chat UI to real LLM backend | 1-2 hours |
| 8.2 | Gather healthcare plan documents for training data | Varies |
| 8.3 | Fine-tune model on plan-specific Q&A | Hours |
| 8.4 | HIPAA compliance review | Varies |
| 8.5 | Deploy to Jenkins Health Insurance website | 2 hours |

---

## 📡 SCOUT-SYSTEM — Shared Bridge With Matthew 🆕

**Repo:** [shuwalker/scout-system](https://github.com/shuwalker/scout-system)
**What:** CSUSB campus job + scholarship discovery pipeline. Multi-agent Python system.

**How Hermes can contribute:**
- Dashboard UI improvements
- README + documentation
- "Opportunity of the week" content generation for JDD
- Scholarship application tracking

### 🐣 Baby Steps

| # | Task | Time |
|---|------|------|
| 9.1 | Hermes reviews scout-system codebase | 30 min |
| 9.2 | Contribute documentation improvements | 1 hour |
| 9.3 | Build campus opportunity → JDD video pipeline | 2 hours |

---

## 🧱 SUPPORTING PROJECTS

### 🔴 IN PROGRESS

| Project | Status |
|---------|--------|
| **Rack PC migration** | 🔴 Blocked — needs Matthew's access |
| **Spiral on Discord server** | 🔴 Blocked — needs Matthew to invite |
| **SSH key on GitHub** | 🔴 Blocked — needs you at PC to paste key |

### 🟡 PLANNED

| Project | Difficulty | Why |
|---------|------------|-----|
| **Hermes Craft** | Med-Hard | Minecraft server AI admin |
| **Elote_Dreamin (Roblox)** | Medium | Cooking tycoon — agent-assisted dev |
| **VR Music Teacher** | Hard | Vision + instruction testbed for Step 4 |
| **MTG Deck Oracle** | Medium | AI Commander deck advisor |

### 💡 SOMEDAY

| Project | Why |
|---------|-----|
| **Home server / cyber deck** | My own JARVIS infrastructure |
| **Eden Glasses** | Step 4 endgame — vision hardware |
| **Hourhand → JDD Portfolio** | ✅ Done — live at HourhandWebsite repo |
| **BeneathArcantum** | ✅ Done — README written, story told |

---

## 📊 THE FULL BOARD

| Status | Count | Items |
|--------|-------|-------|
| ✅ Done | 7 | Lore Bot, MTG Tool, 2 game jams, optimization, Discord DM, Portfolio, BeneathArcantum README |
| 🔴 Blocked | 3 | Rack PC, Spiral invite, SSH key |
| 🐣 Baby Steps | 45+ | Tasks across 9 categories |
| 🟡 Planned | 4 | Hermes Craft, Elote, VR Music, MTG Oracle |
| 💡 Someday | 2 | Home server, Eden glasses |

---

## 🥇 THIS WEEK — Actually Doable

| Day | Task | Time |
|-----|------|------|
| **RIGHT NOW** | 📸 Send photo on Discord — test vision (4.1) | 1 min |
| **RIGHT NOW** | 🎤 Send voice note on Discord (2.1) | 2 min |
| **RIGHT NOW** | 🤖 Test smart home: "Hermes, turn off lights" (5.1) | 2 min |
| **Today** | 📋 Text Matthew: "add Spiral to server + rack PC access pls" (1 + 6.1 + 6.2) | 2 min |
| **Today** | 🔑 Paste SSH key at github.com/settings/ssh/new | 1 min |
| **Tomorrow** | 🐍 `pip install SpeechRecognition pyttsx3 pyaudio` (2.2-2.3) | 1 hour |
| **Wed** | 🔄 Build Jarvis Zero voice loop (2.4) | 1 hour |
| **Thu** | 📡 Learn SSH + networking basics (1.1-1.2) | 30 min |
| **Fri** | 🎥 Create JDD YouTube channel (7.1) | 1 hour |

**Total this week: ~4 hours. Output: Vision tested, voice tested, Jarvis Zero talking, SSH learned, YouTube channel created, Spiral+Ares connected.**

---

*North Star: Hermes as JARVIS. Every project is a step.*
*Last updated: May 28, 2025*
*Next actions: Text Matthew re: Spiral + rack PC. Paste SSH key. Send me a photo.*
