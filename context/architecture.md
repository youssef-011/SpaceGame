# Architecture Notes

Astral should use simple Unity architecture that favors composition, clear ownership, and small reusable components.

## Guiding Principles

- Understand existing systems before adding new ones.
- Prefer composition over inheritance.
- Keep scenes lightweight.
- Keep scripts focused on one responsibility.
- Use events to reduce tight coupling when appropriate.
- Avoid singleton abuse.
- Avoid static state unless there is a clear reason.
- Use ScriptableObjects when they reduce duplication or make tuning easier.
- Create reusable prefabs for repeated gameplay objects.

## Expected System Areas

Future implementation work will likely grow around these areas:

- Player movement and ability state
- Input handling with Unity's New Input System
- Health, damage, and respawn
- Checkpoints
- Simple enemy behaviors
- Traps and hazards
- Collectible or readable story pieces
- Chapter and scene flow
- UI feedback
- Audio triggers

These are planning categories, not permission to implement them during bootstrap.

## Unity Guidelines

- Use Unity 6.
- Use the New Input System.
- Avoid unnecessary packages.
- Keep project dependencies intentional and minimal.
- Prefer serialized configuration over hard-coded values when values need tuning.

## Feature Implementation Rule

Each future feature should start by checking the current architecture and reusing existing patterns. Add abstractions only when they solve a real maintenance problem.
