---
name: create-endpoint
description: Create a CRUD endpoint resource end to end, following project conventions. Use when adding a new resource that needs create/read/update/delete over an in-memory store.
---

# Create Endpoint

Empaqueta el prompt `scaffold-resource` y las reglas `project-conventions` en un procedimiento repetible.

## When to use

Cuando añades un recurso nuevo que necesita endpoints CRUD sobre un store en memoria.

## Inputs

- Resource name (singular).
- Fields with their types.

## Steps

1. Load the `project-conventions` rules.
2. Run the `scaffold-resource` prompt with the resource name and fields.
3. Verify in one short loop: create one item, then list it.
4. Commit: `feat({resource}): scaffold CRUD`.

## Output

A runnable resource with create/read/update/delete backed by an in-memory store.
