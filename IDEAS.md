# 💡 IDEAS.md

> *"The graveyard is the richest place on earth — it's filled with ideas that were never brought to life."*

These are projects I actually want to build. Not tutorial clones, not assignments — real ideas with real vision. When I come back to one, this doc saves me from starting from zero.

---

## 🌽 Elote_Dreamin — Elote Tycoon Simulator

**Platform:** Roblox  
**Genre:** Cooking tycoon / simulator (Papa's Pizzeria-style)  
**Difficulty:** Medium

### The Vision
A street food tycoon where you run an elote cart and build an empire. Start with a single cart on a sidewalk — grill the corn, slather on mayo, sprinkle cheese, chili, lime. Serve customers, earn cash, upgrade your cart. Eventually open a restaurant, then a chain. The comedy writes itself — elote is inherently funny, the toppings are infinite, and nobody's done this on Roblox.

### Core Loop
1. Take order (customer wants: corn + mayo + cheese + extra chili + lime wedge)
2. Grill the corn (timing minigame — don't burn it)
3. Apply toppings in correct order and quantity
4. Serve before patience runs out
5. Earn tips, upgrade cart/ingredients/unlock new toppings

### Why Roblox Over Unity
- Multiplayer built-in (friends can visit your cart/restaurant)
- Currency & shop system already exists
- Avatar system — no character modeling needed
- Tycoon/simulator is a proven genre on the platform
- Players already understand the UI patterns

### Stretch Goals
- Seasonal events (elote for Day of the Dead, Christmas tamales crossover)
- Street cart vs food truck vs restaurant progression
- Compete with rival elote vendors (NPC or PvP)
- Secret menu items unlocked by experimentation

---

## 🎸 VRMusicTeacher — Real Instrument Training in VR

**Platform:** Meta Quest (Unity + XR Interaction Toolkit)  
**Genre:** Music education / rhythm game  
**Difficulty:** Hard (hand tracking is the bottleneck)

### The Vision
Guitar Hero teaches you to press colored buttons. This teaches you to play actual instruments. Put on a Quest headset, look down, and see a virtual guitar/bass/drums with real strings and frets. The game shows you where to place your fingers for actual chords, you strum/pluck with your other hand, and it hears you via the headset mic or a connected instrument to verify you're playing right.

### Why It's Different
| Guitar Hero / Beat Saber | This |
|--------------------------|------|
| Colored buttons | Actual chord shapes |
| Teaches rhythm only | Teaches real instrument skills |
| Transferable skill: zero | Transferable skill: actual guitar |
| "I'm good at a video game" | "I learned guitar" |

### Core Loop
1. Select song + difficulty (beginner chords → full songs)
2. Virtual fretboard shows chord shape with finger positions
3. Strum hand tracks strumming motion
4. Audio recognition confirms correct notes (or just trust the player for v1)
5. Progress through increasingly complex chord progressions

### Tech Challenges
- **Hand tracking accuracy** — Quest 3 is much better but individual finger tracking for frets is still hard. v1 could use controllers as a fallback (grip button = hold string, face buttons = fret positions)
- **Audio recognition** — pitch detection on headset mic is noisy. Could connect via USB audio interface or skip recognition entirely for v1 and just trust the player
- **Latency** — any delay between hand motion and visual feedback kills the feel. Target <20ms

### Scope Down Options
- Start with bass (fewer strings, slower songs)
- Single-chord song mode (play along, no scoring)
- Drum mode first (no fret tracking, just stick tracking)

### Inspiration
- Rocksmith (flat screen, real guitar required)
- Paradiddle (VR drumming, actually works well)
- Pistol Whip (proves rhythm + motion tracking works in VR)

---

## ⛏️ Hermes Craft — Minecraft Server × AI Agent

**Platform:** Minecraft Java Edition + Hermes Agent  
**Genre:** Sandbox / automation  
**Difficulty:** Medium-Hard

### The Vision
A Minecraft server where Hermes acts as an admin/assistant — spawning structures, managing players, running events, generating lore, responding to in-game chat. Imagine saying "build me a castle with a moat" in Minecraft chat and Hermes uses WorldEdit/commands to actually do it.

### Core Loop
1. Player sends chat message → Hermes receives via server plugin
2. Hermes interprets request, generates commands
3. Commands execute on server via RCON or plugin API
4. Hermes responds in chat with personality

### Previous Attempt
Tried on Matthew's rack PC but hit lag issues. The server plus Hermes plus Minecraft was too much. Need optimization.

### Path Forward
- Run Hermes on separate machine from Minecraft server
- Use a lightweight model for real-time chat responses (qwen2.5-coder:7b local)
- Batch build commands instead of executing one at a time
- Use Hermes cron jobs for scheduled server events (nighttime boss spawns, daily challenges)

### Stretch Goals
- AI-generated quests with procedurally spawned dungeons
- Lore bot that remembers player history and builds a narrative
- Auto-builder that translates "build a village" into a series of WorldEdit commands
- Players can vote on what Hermes builds next

---

## 🃏 MTG Deck Oracle — AI-Powered Commander Advisor

**Platform:** Web app / Discord bot  
**Genre:** TCG tool  
**Difficulty:** Medium

### The Vision
My moxfield-deck-color-analyzer proved I can work with MTG data. What if Hermes could analyze your Commander deck and suggest cuts, adds, combos, and power level? Connect to Moxfield/Archidekt API, pull a decklist, run it through an LLM with knowledge of EDHREC, Scryfall, and format meta.

### Why It's Cool
- Every Commander player has "can you look at my deck?" anxiety
- An AI that actually understands synergy and card interactions is genuinely useful
- Could be a Discord bot — join a server, paste a decklist URL, get analysis

### Core Loop
1. User submits Moxfield/Archidekt URL
2. Fetches full decklist + card data from Scryfall
3. Analyzes: curve, color pie, ramp, draw, removal, win conditions
4. Compares against EDHREC data for the commander
5. Returns: power level estimate, suggested cuts (10 cards), suggested adds (10 cards), combo identification

### Tech Stack
- Python (Scryfall API, Moxfield API)
- Hermes Agent for LLM analysis
- Discord bot wrapper (optional)

---

## 🗿 Unfinished Projects I Could Revive

| Project | Status | What's Left |
|---------|--------|-------------|
| **HourhandWebsite** | 4 pages done | Needs finishing touches, README, deploy |
| **ChatGPTWebpageDemo** | Working demo | Polish, make it actually useful |
| **BeneathArcantum** | "game done?" | Your commit literally had a question mark. Figure out what "done" means. |

---

*Last updated: May 25, 2025 — added Elote_Dreamin and VRMusicTeacher after repo cleanup*
*Next: pick one and actually build it. Not start. Build.*
