# Arcadia Core Architecture

## Overview
`arcadia-core` implements an ECS (Entity-Component-System) model, focusing on flexibility, modularity, and performance. It is the base layer for both client and server.

## Major Concepts
- **EntityManager** – Manages creation and deletion of entities
- **Components** – Lightweight data containers
- **Systems** – Behavior applied to matching entities

## Current Systems
- `PhysicsSystem` applies velocity to entities with a `VelocityComponent`.

## Planned
- `RenderSystem`
- `AnimationSystem`
- `SpatialGridSystem`