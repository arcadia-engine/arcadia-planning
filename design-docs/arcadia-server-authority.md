# 🌐 Arcadia Server Authority

This spec defines the multiplayer model for server-side entity simulation, player sync, and authoritative control.

---

## 🎯 Goal

- Server controls "truth" of world state
- Clients send intents (inputs), receive world diffs
- Deterministic simulation supports rollback, prediction

---

## 🔗 ArcadiaConnection Abstraction

All multiplayer traffic routes through:

```java
interface ArcadiaConnection {
    void send(Object message);
    void onReceive(Object message);
}
```

Subtypes:
- `ArcadiaClient`
- `ArcadiaServer`

---

## 🔁 Tick Sync

### Server
- Simulates physics, movement, AI
- At `n` ms intervals, sends state diffs:
```json
{
  "entityId": "abc123",
  "component": "PositionComponent",
  "data": { "x": 5, "y": 3 }
}
```

### Client
- Receives updates
- Optionally predicts or interpolates frames

---

## 🧠 Authority Model

| Concept | Description |
|--------|-------------|
| Input Intent | Client sends player action (W, attack, use) |
| State Sync | Server sends updated entity state (position, health) |
| Interpolation | Client smooths updates between syncs |
| Prediction | Client guesses outcome before server confirms |

---

## 🧩 Future Features

- Lag compensation
- Server rewind validation
- Out-of-sync detection
