# Arcadia – Idea Backlog

## Mechanics
- Tether system for mob AI chaining
- Fog of war reveal by region
- Multi-layered world tiles (underground, elevation)

## Technical
- Hot-reload system for tileset configuration
- In-game mod toolkit with JSON schema validator
- Entity save/load using a binary blob

## UI
- Command palette like VSCode for dev commands
- Right-click context menu for tiles/entities

### Current Systems
- `PhysicsSystem`: Applies velocity to entities with a `VelocityComponent`
- `RenderSystem`: Renders static ASCII grid for entity positions
- `EngineLogger`: Provides timestamped, stylized logs across all systems
