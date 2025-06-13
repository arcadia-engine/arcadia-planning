# 🖼️ Arcadia Client UI

This spec outlines the philosophy and architecture for the client-facing UI layer in Arcadia. The UI will be modular, data-driven, and renderer-agnostic.

---

## 🎨 UI Zones

- **Top HUD**: Health, stamina, mana, etc.
- **Bottom HUD**: Dialog boxes, controls
- **Minimap**: (optional)
- **Overlay**: Contextual prompts, damage numbers

---

## 🔧 UI System

The `UISystem` is injected into the `GameLoop` like any other logic system:

```java
app.registerSystem(new UISystem());
```

It handles:
- Frame-by-frame HUD drawing
- Interpolated overlays
- Text and symbol rendering via `Renderer`

---

## 🧾 JSON UI Definition (Planned)

```json
[
  {
    "type": "label",
    "text": "Health: ${player.hp}",
    "x": 1,
    "y": 22,
    "color": "red"
  }
]
```

- Bindings use `${}` to interpolate entity or game state
- Assets defined in external files

---

## 🔮 Future Features

- Layout managers (grid, stack, absolute)
- Dynamic fade-in/out
- Renderer abstraction for GUI/ASCII

---

## 💡 Notes

UI does not own state—only renders it. Entity and system data remain in the simulation layer.
