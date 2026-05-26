# 📋 PROJECTS.md — Building JARVIS

> *"Ideas are cheap. Execution is aura."*
> *North Star: Hermes as a JARVIS/EDEN-grade assistant — always listening, everywhere, sees what I see.*

---

## 🧭 THE VISION — Hermes as JARVIS / EDEN

This is why every other project on this board exists. Every commit, every repo, every skill is a brick in this wall.

| JARVIS Trait | What It Means | Our Status |
|-------------|---------------|------------|
| 🗣️ Always listening, voice-first | Wake word → Hermes responds anywhere | 🟡 Planned |
| 📱 Everywhere — all devices | Phone, desktop, Discord, glasses | 🟢 Works on Discord/CLI |
| 🏠 Controls the house | Smart home (lights, music, automation) | ✅ Hue set up |
| 👁️ Sees what you see | Camera → Hermes vision in real-time | 💡 Someday |
| 🧠 Remembers everything | Cross-device memory and session continuity | 🟢 Active |
| ⚡ Reacts instantly | Local model for fast, cloud for smart | 🟢 Active (multi-provider) |
| 🏗️ Can build things | MC server, APIs, 3D printing, automation | 🟡 Planned |

---

## 🎯 THE JARVIS ROADMAP (in order)

```
Step 1 ──→ Step 2 ──→ Step 3 ──→ Step 4 ──→ Step 5
Server    Voice     Devices   Vision    Smart Home
```

### Step 1: 🖥️ The Brain — A 24/7 Server
**Status:** 🔴 BLOCKED (needs Matthew's rack PC access)

Hermes can't be JARVIS if it only runs when my gaming PC is on. Needs a permanent home.

| Option | Pros | Cons |
|--------|------|------|
| Matthew's rack PC (now) | Already running 24/7, has MC server | Need access, shared resource |
| My own home server (later) | Total control, my hardware | $$$, setup time |
| Cloud VPS | Zero hardware, instant | Monthly cost, privacy |

**Done:** Migration plan written, rack-pc-migration skill created. Just need access.

### Step 2: 🎤 Always Listening — Voice Wake Word
**Status:** 🟡 No technical plan yet

"Hey Hermes" → session opens → voice conversation. Not typing. Real JARVIS energy.

| Approach | Difficulty | Notes |
|----------|------------|-------|
| Phone always-listening widget | Medium | Most practical start |
| Desktop mic + wake word daemon | Medium | openWakeWord or Porcupine |
| Dedicated mic hardware | Hard | Raspberry Pi + mic array |

**Goal:** "Hey Hermes" on my phone, instantly get a voice response. Discord already solves the delivery — this is about the input.

### Step 3: 📱 Every Device — True Omnipresence
**Status:** 🟢 Discord (partial), 💡 native app (future)

| Device | Status | How |
|--------|--------|-----|
| Desktop WSL | ✅ CLI + Discord | Already works |
| Phone (iPhone) | ✅ Discord DM | Works now |
| MacBook | 💡 Not set up | Same Discord — just log in |
| Glasses / wearable | 💡 Eden glasses project | Hardware build |
| Car / speakers | 💡 Bluetooth voice | Future |

### Step 4: 👁️ The Eyes — Hermes Sees What You See
**Status:** 💡 Eden Glasses project

This is the dream. Point at something and Hermes knows what you're looking at.

| Phase | Approach | Difficulty |
|-------|----------|------------|
| Phase 0: Phone camera | iPhone camera → Discord image → Hermes vision | Easy — works NOW |
| Phase 1: Hack existing | Meta Ray-Bans + API | Medium, $300-400 |
| Phase 2: DIY glasses | Raspberry Pi + camera + display + audio | Hard, $100-200 |
| Phase 3: Custom Eden glasses | 3D printed frame + custom PCB + optics | Very Hard |

**Start with Phase 0 TODAY.** Open Discord on your phone, take a photo, send it to Hermes. "What am I looking at?" — instant vision. The glasses make it ambient but the core functionality is already here.

### Step 5: 🏠 The House — Smart Home Control
**Status:** 🟡 Philips Hue connected, needs Hermes wiring

Philips Hue is already set up via OpenHue. Hermes can already control lights. Expand to:
- Music (Spotify integration)
- Climate (if smart thermostat exists)
- Routines ("goodnight" → lights off + gateway pause + phone DND)

---

## 🧱 BUILDING BLOCKS (existing projects that feed JARVIS)

### ✅ Already Done

| Project | JARVIS Connection |
|---------|-------------------|
| Discord DM setup | Hermes on phone — the "everywhere" piece |
| Gaming mode | Hermes knows when to be quiet — JARVIS etiquette |
| Multi-provider config | Fast local + smart cloud — the JARVIS brain model |

### 🔴 Next Up

| Project | JARVIS Connection |
|---------|-------------------|
| Rack PC migration | The 24/7 server — Step 1 |

### 🟡 Planned

| Project | JARVIS Connection |
|---------|-------------------|
| Hermes Craft | Hermes controls a digital world — the "build things" muscle |
| Elote_Dreamin | A project Hermes can help build — agent-assisted game dev |
| VR Music Teacher | Hermes sees your hands and teaches — vision + instruction testbed |
| MTG Deck Oracle | Hermes analyzes and explains complex systems — the "smart" piece |

### 💡 Someday

| Project | JARVIS Connection |
|---------|-------------------|
| Home server / cyber deck | My own JARVIS hardware — total control |
| Eden Glasses | The eyes — vision anywhere |
| HourhandWebsite | Portfolio to show off the JARVIS project |
| BeneathArcantum | Finish something — momentum |

---

## 📊 THE FULL BOARD

| Status | Count | Projects |
|--------|-------|----------|
| ✅ Done | 6 | Lore Bot, MTG Analyzer, 2 game jams, optimization, Discord DM |
| 🔴 Next Up | 1 | **Rack PC migration** ← unblock this |
| 🟡 Planned | 4 | Hermes Craft, Elote Tycoon, VR Music, MTG Oracle |
| 💡 Vision | 5 | Voice wake word, every device, Eden glasses, smart home, 24/7 server |

---

## 🥇 RIGHT NOW — What You Can Do Today

1. **Test Hermes vision on phone:** Discord DM → send photo → "what do you see?"
2. **Try a voice message:** Discord voice note → Hermes responds
3. **Ask Matthew for rack PC access** — unblock Step 1
4. **Play with Hue lights:** "Hermes, dim the lights" (it already works)

---

*Last updated: May 25, 2025*
*North Star: Hermes as JARVIS. Every project is a step.*
*Next action: Unblock rack PC migration (Step 1 of JARVIS roadmap).*
