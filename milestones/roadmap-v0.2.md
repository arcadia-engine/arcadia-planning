# 🛠️ Arcadia Engine Roadmap (v0.2–v0.5)

---

## 🔹 v0.2 – Demo Zone Foundations
> Goal: A playable offline sandbox with real entity interaction and screen-based feedback.

### ✅ Milestone Goals
- [ ] `CollisionSystem` for static object blocking  
- [ ] `HealthComponent` and damage model stub  
- [ ] `UISystem` for HUD display (health, coords, FPS)  
- [ ] `TileMapLoader` – ASCII tile map definition + parsing  
- [ ] `InteractionSystem` (signs, doors, etc.)

### 📅 Target Date
**June 30, 2025**

> Ends with a working single-player test zone, player + NPC interaction, and no network required.

---

## 🔹 v0.3 – Simulation Layer Maturity
> Goal: Core mechanics like combat, inventory, and AI.

### ✅ Milestone Goals
- [ ] `CombatSystem` (damage on proximity or input)  
- [ ] `InventoryComponent` + sample `ItemComponent`  
- [ ] `AIBrainSystem` (wander, chase, idle)  
- [ ] `DeathSystem` (entity removal on 0 HP)  
- [ ] `SaveSystem` (serialize entities to JSON)

### 📅 Target Date
**July 14, 2025**

> Ends with a local dungeon-style test, inventory working, AI/NPC behaviors enabled.

---

## 🔹 v0.4 – Networking Alpha
> Goal: Local server-client multiplayer simulation.

### ✅ Milestone Goals
- [ ] `ClientNetSystem` (send `InputIntentPacket`)  
- [ ] `ServerNetSystem` (receive + apply, then sync position)  
- [ ] `EntitySpawnPacket` + dynamic sync  
- [ ] `StateSnapshotPacket` broadcasting loop  
- [ ] Server-side `GameLoop` separation

### 📅 Target Date
**July 28, 2025**

> Ends with player input over TCP + visible position sync between host and client.

---

## 🔹 v0.5 – World Server Demo
> Goal: Simulated MMO backend slice with real-world updates and authority.

### ✅ Milestone Goals
- [ ] Remote player entities with visible separation  
- [ ] Server-authoritative spawns (e.g., monster AI)  
- [ ] Entity UUID map and lifetime sync  
- [ ] Server logs + profiling tools  
- [ ] First full-stack play session (1v1 combat, sync + confirm)

### 📅 Target Date
**August 11, 2025**

> Ends with your first working multiplayer “arena” experience and data-correct network sync.
