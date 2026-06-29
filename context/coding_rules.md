# Coding Rules

## C# Style

- Use standard C# naming conventions.
- Use PascalCase for classes, methods, properties, and public members.
- Use camelCase for private fields and local variables.
- Prefer `[SerializeField] private` fields over public fields in Unity components.
- Keep one class focused on one responsibility.
- Avoid scripts larger than about 300 lines unless there is a clear reason.

## Unity Code

- Keep MonoBehaviours small and readable.
- Separate input, movement, combat, health, and UI responsibilities when practical.
- Prefer inspector-configurable values for gameplay tuning.
- Use prefabs for reusable gameplay objects.
- Use ScriptableObjects for shared configuration when useful.
- Avoid hidden dependencies between scene objects.

## Collaboration

- Do not introduce features outside the requested task.
- Do not duplicate systems that already exist.
- Keep naming consistent with the project.
- Favor readable code over clever code.
- Add comments only when they clarify non-obvious intent.

## Quality Bar

Every gameplay failure should feel fair and teach the player something. Code should follow the same spirit: simple, explicit, and easy to reason about.
