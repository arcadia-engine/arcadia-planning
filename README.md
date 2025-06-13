# 🧠 Arcadia Planning

**Arcadia Planning** is the command center for the [Arcadia Engine](https://github.com/arcadia-engine) ecosystem—a modular Java engine for creating 2D simulations, roguelikes, and MMO-scale games.

This repo tracks the design, structure, and development lifecycle of Arcadia across all core modules: `arcadia-core`, `arcadia-client`, `arcadia-server`, `arcadia-net`, `arcadia-tools`, and `arcadia-demo`.

---

## 🚀 Purpose

This is where the **philosophy becomes structure**.

Arcadia Planning serves as:
- 📓 A live **devlog archive**
- 📘 A set of detailed **specification docs**
- 🗺 A milestone-driven **roadmap**
- 🧱 A foundation for all contributors and future expansion

---

## 🧭 Navigation

### 📖 Devlogs
Time-stamped progress notes, session breakdowns, and refactors.

- [`devlogs/`](./devlogs)

### 📐 Specs
Technical deep dives for core systems (e.g. `ArcadiaApp`, `TileMapLoader`, `Networking`).

- [`specs/`](./specs)

### 📅 Milestones & Roadmap
Development phases and version targets.

- [`milestones/roadmap-v0.1.md`](./milestones/roadmap-v0.1.md)
- [`milestones/roadmap-v0.2.md`](./milestones/roadmap-v0.2.md)

### 📂 Archive (Optional)
Old notes and design thoughts for future reference.

- [`archive/`](./archive)

---

## 🧱 Active Modules

| Module | Purpose |
|--------|---------|
| [`arcadia-core`](https://github.com/arcadia-engine/arcadia-core) | ECS engine, runtime logic, system pipeline |
| [`arcadia-client`](https://github.com/arcadia-engine/arcadia-client) | Input, rendering, UI |
| [`arcadia-server`](https://github.com/arcadia-engine/arcadia-server) | Headless multiplayer server |
| [`arcadia-net`](https://github.com/arcadia-engine/arcadia-net) | Client/server communication layer |
| [`arcadia-demo`](https://github.com/arcadia-engine/arcadia-demo) | Example implementation of a 2D sandbox |


---

## 🧠 Arcadia Manifesto

> Simulation before sensation.  
> Logic before light.  
> Build worlds that can think before they shine.

Arcadia is about empowering control through architecture. It’s not a toy engine—it’s a system builder’s playground.  
Every component is modular. Every loop is yours to own. The engine just helps you run it cleanly.

---

## 🔜 What's Next?

- Integrate `TileMapLoader` and file-based map definitions  
- Build `SystemManager` for runtime system registration/order  
- Begin networking layer (`ArcadiaConnection`, `ArcadiaClient`, `ArcadiaServer`)  
- Add `AnimationSystem` for 2D sprite logic  
- Expand devlogs and specifications for contributors

---

MIT Licensed · Built with Java 17 · Maintained by [Hemerley](https://github.com/Hemerley)
