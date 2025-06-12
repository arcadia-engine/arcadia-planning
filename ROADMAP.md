# 🛠 Arcadia Engine: Master Roadmap

The Arcadia Engine is a modular, tile-based 2D game engine and demo MMO world built using Java.

This roadmap tracks the development of all major modules:

---

## 🎯 Goal

Build a modular, multiplayer-ready 2D game engine capable of powering RPGs, roguelikes, and online experiences.

---

## 🧱 Core Modules

### ✅ `arcadia-core`
- [ ] Entity-Component System (ECS)
- [ ] Game loop (tick-based)
- [ ] Input manager
- [ ] Tile + animation engine
- [ ] Save/load system
- [ ] Resource loader (JSON or binary)

### 🚀 `arcadia-client`
- [ ] Render tilemaps + entities
- [ ] Camera control + zoom
- [ ] UI framework (inventory, hotbar, dialog)
- [ ] Audio playback (FX + ambient)

### 🧠 `arcadia-server`
- [ ] Login/handshake protocol
- [ ] Player position sync
- [ ] Mob AI logic
- [ ] Zone triggers / events
- [ ] Server commands + admin tools

### 🛠 `arcadia-tools`
- [ ] Visual map editor (tile + object layers)
- [ ] Entity prefab editor (JSON)
- [ ] Dialogue/quest builder
- [ ] Mod loader + packager

### 🌍 `arcadia-demo`
- [ ] Starter zone (village)
- [ ] NPCs + combat
- [ ] Leveling and loot
- [ ] Dialog, quests, and cutscenes

### 📚 `arcadia-docs`
- [ ] Architecture overview
- [ ] Getting started guide
- [ ] Build + contribution instructions
- [ ] Devlogs + changelogs
- [ ] GitHub Pages deployment

---

## 🧭 Milestones

| Phase          | Focus                            | ETA         |
|----------------|----------------------------------|-------------|
| **Phase 1**    | Core loop, ECS, rendering        | Aug 2025    |
| **Phase 2**    | Networking, client/server sync   | Dec 2025    |
| **Phase 3**    | Tooling + playable demo zone     | Mar 2026    |
| **Phase 4**    | Polish + docs + deployable build | Summer 2026 |

---

## 📎 Contributions

This project is currently maintained by [@Hemerley](https://github.com/Hemerley).  
External contributions will be welcome once phase 2 begins.

MIT Licensed · Java 17+ · Built with love
