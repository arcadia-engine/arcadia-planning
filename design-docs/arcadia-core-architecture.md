# 🧱 Arcadia Core Architecture

Arcadia Core is the foundational module that powers the Arcadia Engine’s ECS framework. It is responsible for orchestrating the simulation of game logic through systems, components, and a fixed-timestep game loop.

---

## 🔄 Architecture Overview

```
ArcadiaApp
   └── Scene
       └── GameLoop
           └── System Pipeline
```

This decoupling ensures plug-and-play flexibility across terminals, GUI layers, and multiplayer backends.

---

## 🔧 Core Components

### 🧠 Entity-Component-System (ECS)
- `Entity`: Unique game object ID
- `Component`: POJO data container (no logic)
- `EntityManager`: Registry managing entity lifecycles and component access
- `GameSystem`: Executes logic each tick on matching entities

### 🌀 GameLoop
- Runs at fixed timestep (default 60 FPS)
- Injected with list of `GameSystem`s
- Accepts `Renderer`, `InputProvider`, and entity state

### 🧱 Scene
- Loads and populates entities
- Owns `MapManager` (or later: world state)
- Interacts with core via `load(EntityManager)`

---

## 🚀 ArcadiaApp

> The public runtime interface for developers using Arcadia.

- Simplifies initialization, rendering, system registration, and scene management
- Example:

```java
ArcadiaApp app = new ArcadiaApp()
  .setRenderer(new LanternaRenderer(screen))
  .setInputProvider(new LanternaInputProvider(screen))
  .registerSystem(new PhysicsSystem(map))
  .loadScene(new DemoScene())
  .run();
```

---

## 📦 Engine Modules (Planned)

| Module | Purpose |
|--------|---------|
| arcadia-core | ECS + simulation engine |
| arcadia-client | Input/render layers |
| arcadia-net | Networking & sync layer |
| arcadia-server | Server tick + authority logic |
| arcadia-tools | Editor & utilities |

---

## 🧩 Future Enhancements

- Runtime `SystemManager`
- File-based map and entity loader
- Priority-ordered system execution
- Deterministic replays and save states
