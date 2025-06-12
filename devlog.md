# 📜 Arcadia Engine – Development Log

> Ongoing updates, reflections, and milestones on the creation of the Arcadia Engine — a modular, open-source game engine built in Java.

---

## 📅 Devlog Entry 001 – **Arcadia Begins**
🗓️ **Date**: June 12, 2025  
👤 **Author**: @Hemerley  

### Summary
Today marks the formal creation of the Arcadia Engine GitHub organization and project structure. After years of concept drafts and learning, the foundation for a long-term, modular 2D engine is now real.

**Accomplished:**
- ✅ Created `arcadia-engine` GitHub organization
- ✅ Set up 6 modular repositories:
  - `core`, `client`, `server`, `tools`, `demo`, `docs`
- ✅ Added LICENSE, README.md, and structure for each
- ✅ Established planning repo: `arcadia-planning`
- ✅ Published `ROADMAP.md` and `project-board.md`
- ✅ First visual branding complete (logo + identity)

### Reflection
This is more than just a project—Arcadia represents the shift from dreaming to *building*. Instead of imitating other engines or games, this is about crafting something modular, meaningful, and unique.

Even if it ships with a single zone or single quest, it will be mine. And finished.

---

## 📅 Next Planned Entry
- 🧱 Initial Java scaffolds: `GameLoop`, `Entity`, `Component`
- 🗺 Tile renderer and testbed
- 📐 ECS notes and system outline

---

> *"The world won't build itself. I will."*

## [#002] The Engine Breathes — Movement, Systems, and Logs
🗓️ June 12, 2025

Arcadia Engine is no longer static.

Today marks the completion of our ECS-driven movement loop. The old imperative update logic has been fully replaced by cleanly separated `System` classes, starting with `PhysicsSystem`. Entities now move across the simulated world using component-based velocity data, applied independently of the core loop.

### ✅ What's Working
- `Entity`, `Component`, `EntityManager`, and `GameSystem` interfaces are live
- `PositionComponent` and `VelocityComponent` fully drive movement
- `PhysicsSystem` applies velocity per tick to simulate motion
- The `GameLoop` uses a fixed timestep (60 FPS) with pluggable systems
- Logging infrastructure added (`EngineLogger`) with:
  - Timestamped messages
  - Log levels: `info`, `debug`, `error`
  - ANSI color-coded output for easy parsing in the terminal

### 🔄 Systems Pipeline Example
[21:10:58] [INFO] [Arcadia] 🌀 Arcadia Engine started...
[21:10:59] [DEBUG] [Arcadia] PhysicsSystem → Entity 84c4... moved to Position(14, 25)


### 🧠 Lessons Learned
- Avoid Java naming collisions (`System` vs `GameSystem`)
- Shadowing variables (like `player`) creates hidden bugs
- ECS encourages clean separation of state and behavior
- Logging is not just a utility—it's visibility

### 🧭 What's Next
- Begin visual output via a `RenderSystem`
- Define tilemaps, grids, and spatial layers
- Draft out the `arcadia-core` package structure to support growth
- Possibly create `EntityFactory` for clean game object creation

Arcadia is no longer theoretical. It ticks, moves, and speaks in code.

