# Scaffold Resource — reusable prompt

Copia este prompt, rellena los placeholders y ejecútalo en un bucle corto.

---

Create a `{ResourceName}` resource with these fields:

```
{fieldName}: {type}
{fieldName}: {type}
```

Requirements:
- Expose CRUD endpoints: create, read one, read all, update, delete.
- Back it with a single in-memory store that persists within the session.
- Follow the project conventions already in place.
- Keep it runnable: I will create one item and list it right after.

---

> Example fill: `ResourceName = Rocket`, fields `name: text`, `seatCapacity: integer`, `operationalRange: integer`.
