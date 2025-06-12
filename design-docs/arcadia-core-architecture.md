# Arcadia Core Architecture

## Overview
`arcadia-core` implements an ECS (Entity-Component-System) model, focusing on flexibility, modularity, and performance. It is the base layer for both client and server.

## Major Concepts
- **EntityManager** – Manages creation and deletion of entities
- **Components** – Lightweight data containers
- **Systems** – Behavior applied to matching entities
- 
### Current Systems
- `PhysicsSystem`: Applies velocity to entities with a `VelocityComponent`
- `RenderSystem`: Renders static ASCII grid for entity positions
- `EngineLogger`: Provides timestamped, stylized logs across all systems

## Planned
- `RenderSystem`
- `AnimationSystem`
- `SpatialGridSystem`
