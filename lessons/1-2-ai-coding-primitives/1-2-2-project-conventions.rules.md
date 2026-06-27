---
name: project-conventions
description: Always-on conventions for AstroBookings resources.
alwaysApply: true
---

# Project conventions

- Group each resource together: endpoint, model and store in one folder.
- Name endpoints by resource in plural; name the model in singular.
- Persist data within the session using one in-memory store per resource.
- Validate input at the endpoint boundary and return a clear, consistent error shape.
- Keep every change runnable: each resource must be creatable and listable.
- Keep names explicit and intention-revealing; no abbreviations.
