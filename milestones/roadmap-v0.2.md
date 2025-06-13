# 🛣 Arcadia Engine Roadmap – v0.2

> Target: Playable offline sandbox with real entity interaction, pluggable scenes, and map loading

---

## 🧩 Runtime Architecture

- [x] `ArcadiaApp` for developer-facing engine interface
- [x] `Scene` interface for game state management
- [x] Refactored `GameLoop` for injection-based lifecycle
- [x] Modular demo using `DemoScene`

---

## 🌍 World Simulation

- [x] MapManager and Tile/TileType abstractions
- [ ] Move map classes into `arcadia-core`
- [ ] Implement `TileMapLoader` for ASCII or JSON maps
- [ ] Add Viewport/Camera support for scrollable scenes

---

## ⚙️ System Improvements

- [x] InputSystem and PhysicsSystem
- [x] RenderSystem using layer + tile drawing
- [ ] `SystemManager` for runtime-controlled system order and injection
- [ ] Add `UISystem` for healthbars, messages, etc.

---

## 🔄 Animation & Visual Feedback

- [ ] Create `AnimationComponent` and `AnimationSystem`
- [ ] Support sprite frame switching based on ticks or state

---

## 🌐 Networking Scaffold

- [ ] Define `ArcadiaConnection` abstraction
- [ ] Implement `ArcadiaClient` and `ArcadiaServer` shell classes
- [ ] Plan sync message format and entity state flow

---

## 🎯 Goal Completion

Ends with:
- Fully functional demo scene
- File-based maps
- Entities reacting to player movement and physics
- Ready to fork into client/server or world editor layers
