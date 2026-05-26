# 📋 PROJECTS.md — What I'm Actually Building

> *"Ideas are cheap. Execution is aura."*

Status key:
- ✅ Done, shipped
- 🔴 Next up (prioritized)
- 🟡 Planned (has a real design doc)
- 💡 Someday (no plan yet)

---

## ✅ COMPLETED

### ⚡ Hermes Instant Lore Bot
**Repo:** [hermes-instant-lore-bot](https://github.com/SeanJ07/hermes-instant-lore-bot)
**Shipped:** May 2025

"Give me lore" → instant free certs, badges, and credentials. Aura factory. Has a Hermes skill attached so I can just ask for certs and get instant answers.

### 🃏 MTG Deck Color Analyzer
**Repo:** [moxfield-deck-color-analyzer](https://github.com/SeanJ07/moxfield-deck-color-analyzer)
**Shipped:** June 2025

Python tool that pulls Moxfield decklists and breaks down color ratios using Scryfall API.

### 🎮 GMTK Game Jam 2024 — Tiny Tim's Big Adventure
**Repo:** [GMTKGameJam2024](https://github.com/SeanJ07/GMTKGameJam2024)

Submitted, built, done. Game jam entry.

### 🚀 Finding Elon
**Repo:** [Finding-Elon](https://github.com/SeanJ07/Finding-Elon)

"Rescue Elon from the evil rember." ASP.NET game. Shipped.

### ⚙️ Hermes Optimization
**What:** Gaming mode / restore mode scripts
**Shipped:** May 2025

`game-mode-v2.sh` kills gateway, unloads Ollama models, caps WSL memory, kills EpicWebHelper + power plan switching. `restore-mode-v2.sh` reverses everything. Hermes `gaming-mode` skill auto-loads on trigger words.

### 📡 Discord DM Setup
**What:** Hermes reachable via Discord DM to "Spiral"
**Shipped:** May 2025

Systemd user service, DM-only, allowlist via DISCORD_ALLOWED_USERS. Works from phone and desktop.

---

## 🔴 NEXT UP (highest priority)

### 🖥️ Rack PC Migration — Move Hermes Off Gaming PC
**Priority:** HIGH
**Difficulty:** Hard
**Blocked by:** Need rack PC IP + SSH access from Matthew

**The Plan:**
1. Deploy Hermes in Docker on rack PC (xmbshwll/hermes-agent-docker or hermeshq)
2. Install hermes-tool-slimmer for lighter prompts
3. Copy over all skills, memory, and config from gaming PC
4. Verify gaming PC lag is gone

**Why:** Hermes on my gaming PC eats RAM and causes lag during games. Rack PC already runs 24/7 with a Minecraft server — Hermes belongs there. My PC becomes a thin client connected through Discord/CLI.

**Done so far:**
- [x] Full migration skill created (`rack-pc-migration`)
- [x] Identified repos/tools needed
- [ ] Get rack PC access from Matthew
- [ ] Deploy

---

## 🟡 PLANNED (have design docs)

### ⛏️ Hermes Craft — AI Minecraft Server
**Platform:** Minecraft Java + Hermes Agent
**Difficulty:** Medium-Hard
**Depends on:** Rack PC Migration

Hermes as a Minecraft server admin — spawn structures, manage players, run events, respond to in-game chat. Eventually: "build me a castle with a moat" and Hermes actually does it.

**Core Features:**
- In-game chat → Hermes interprets → server commands
- Scheduled events via Hermes cron jobs
- AI-generated quests with procedurally spawned dungeons
- Lore bot that remembers player history

**Path Forward:**
- Run on rack PC alongside MC server
- Use lightweight local model (qwen2.5-coder:7b) for real-time responses
- Batch build commands instead of one-at-a-time execution

### 🌽 Elote_Dreamin — Elote Tycoon (Papa's Pizzeria Style)
**Platform:** Roblox
**Difficulty:** Medium

Street food tycoon — start with an elote cart, build a restaurant empire. Grill the corn, add mayo, cheese, chili, lime. Serve customers, upgrade. Nobody's done elote on Roblox and the theme is inherently funny/chaotic.

**Core Loop:** Take order → grill corn (timing minigame) → add toppings → serve → earn tips → upgrade

**Why Roblox:** Multiplayer/economy/avatars built-in. Tycoon genre is proven. No character modeling needed.

### 🎸 VRMusicTeacher — Real Guitar Training in VR
**Platform:** Meta Quest (Unity + XR)
**Difficulty:** Hard

VR app that teaches actual guitar. Not Guitar Hero colored buttons — real chord shapes, real frets, real strumming. See virtual fretboard, place fingers correctly, strum with hand tracking.

**Tech Challenges:**
- Hand tracking accuracy for individual fingers (Quest 3 is better)
- Audio recognition for pitch detection
- Latency <20ms for feel

**Scope Down Options:** Start with bass (fewer strings), or drum mode (no fret tracking).

### 🃏 MTG Deck Oracle — AI Commander Analyzer
**Platform:** Web / Discord bot
**Difficulty:** Medium

Paste a Moxfield deck URL → AI analyzes synergy, curve, combos, power level. Suggests cuts and adds using EDHREC + Scryfall data. Actually useful for every Commander player.

**Tech:** Python (Scryfall/Moxfield APIs) + Hermes for LLM analysis. Optional Discord bot wrapper.

---

## 💡 SOMEDAY (no plan yet, just vibes)

### 🏠 Home Server / Cyber Deck
**What:** Build my own home server rig — custom hardware, possibly a cyber deck form factor (portable retro-futuristic terminal computer)
**Why:** Own my infrastructure. Run Hermes, Minecraft, media server, whatever. Not dependent on Matthew's rack PC or cloud services.
**Brain Dump:** Raspberry Pi? Old laptop? Custom 3D printed case? SBC cluster? No decisions made yet — just the idea of having my own server.

### 🏗️ HourhandWebsite
**Repo:** [HourhandWebsite](https://github.com/SeanJ07/HourhandWebsite) (private)
**Status:** 4 HTML pages done, dark portfolio/storefront vibes. Needs finishing touches, README, deployment.

### 🤖 ChatGPTWebpageDemo
**Repo:** [ChatGPTWebpageDemo](https://github.com/SeanJ07/ChatGPTWebpageDemo)
**Status:** Working demo with multiple HTML pages. Got a responsive redesign. Could polish into something useful.

### 🏰 BeneathArcantum
**Repo:** [BeneathArcantum](https://github.com/SeanJ07/BeneathArcantum) (private)
**Status:** SkillsUSA game project. Last commit: "game done?" — literally has a question mark. Figure out if it's actually done.

---

## 📊 AT A GLANCE

| Status | Count | What |
|--------|-------|------|
| ✅ Done | 6 | Lore Bot, MTG Analyzer, 2 game jams, optimization, Discord |
| 🔴 Next | 1 | Rack PC migration |
| 🟡 Planned | 4 | Hermes Craft, Elote, VR Music, MTG Oracle |
| 💡 Someday | 3 | Home server, Hourhand, ChatGPT demo, BeneathArcantum |

---

*Last updated: May 25, 2025*
*Next action: Get rack PC access from Matthew and ship the migration.*
