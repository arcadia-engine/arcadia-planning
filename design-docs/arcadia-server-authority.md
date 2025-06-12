# Server-Authority Design

## Core Goal
Arcadia is designed with a server-authoritative architecture to maintain game integrity, reduce exploits, and support large-scale multiplayer sessions.

## Responsibilities
- Maintain world state and timing
- Validate client actions
- Push state diffs to clients
- Manage login, persistence, and instances

## Tools
- Java Sockets or Netty (TBD)
- Tick-based logic
- Delta compression (future phase)