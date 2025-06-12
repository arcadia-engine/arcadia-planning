# 📌 Arcadia Engine Project Board

Central tracking board for all work related to the Arcadia Engine suite.  
Tasks are grouped by status and scope.

---

## ✅ STATUS LEGEND

- 🔹 **Backlog** = Planned, not started
- 🔧 **In Progress** = Actively being worked on
- 🧪 **In Review** = Ready to test or submit
- ✅ **Complete** = Done and committed

---

## 🧱 CORE ENGINE (`arcadia-core`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Setup project structure / packages    | 🔧 In Progress | `com.arcadia.core`  
| Implement ECS base classes (Entity, Component, System) | 🔹 Backlog    |  
| Build game loop + tick scheduler      | 🔹 Backlog    |  
| Input handling (keyboard/mouse)       | 🔹 Backlog    |  
| Resource manager (tiles, animations)  | 🔹 Backlog    |  
| Logging and debug tools               | 🔹 Backlog    |  

---

## 🎮 CLIENT (`arcadia-client`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Init render surface + windowing       | 🔹 Backlog    | Using LibGDX or LWJGL  
| Implement basic camera                | 🔹 Backlog    | Follow player center  
| Draw tiles and animated sprites       | 🔹 Backlog    |  
| UI window system                      | 🔹 Backlog    |  
| Inventory + hotbar display            | 🔹 Backlog    |  

---

## 🧠 SERVER (`arcadia-server`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Basic socket server loop              | 🔹 Backlog    | Java NIO or Netty  
| Client handshake / login              | 🔹 Backlog    |  
| Sync player state                     | 🔹 Backlog    |  
| NPC AI system                         | 🔹 Backlog    |  
| Admin command interface               | 🔹 Backlog    |  

---

## 🛠 TOOLS (`arcadia-tools`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Tilemap editor base UI                | 🔹 Backlog    |  
| JSON loader/saver for maps            | 🔹 Backlog    |  
| Entity prefab builder                 | 🔹 Backlog    |  
| Quest/dialogue editor                 | 🔹 Backlog    |  

---

## 🌍 DEMO (`arcadia-demo`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Starter zone tilemap                  | 🔹 Backlog    | Design forest/village  
| Create sample NPCs with quests        | 🔹 Backlog    |  
| Setup sample combat + loot            | 🔹 Backlog    |  
| Build storyline intro                 | 🔹 Backlog    |  

---

## 📚 DOCS (`arcadia-docs`)

| Task                                  | Status      | Notes |
|---------------------------------------|-------------|-------|
| Getting Started Guide                 | 🔹 Backlog    | For new devs  
| Architecture overview                 | 🔹 Backlog    | Visual flow diagrams  
| Devlog template                       | 🔹 Backlog    | Markdown format  
| GitHub Pages setup                    | 🔹 Backlog    |  

---

## 🧭 Timeline Goals

| Phase | Focus                          | Target Completion |
|-------|--------------------------------|-------------------|
| Phase 1 | Core loop + ECS + Rendering     | August 2025       |
| Phase 2 | Networking + Sync + Mob Logic   | Dec 2025          |
| Phase 3 | Tools + Demo World              | March 2026        |
| Phase 4 | Docs + Polish + Showcase        | Summer 2026       |

---

_Updated by [@Hemerley](https://github.com/Hemerley) · Arcadia Engine is an open-source initiative for serious engine development._

