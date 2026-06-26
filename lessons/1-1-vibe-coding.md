---
title: Vibe Coding
description: Iterate in short loops until you get a result.
url: 1-1-vibe-coding
footer: Vibe Coding · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.1 - Vibe Coding

AstroBookings arranca: un esqueleto que ya corre y un `GET /api/health`. Hoy le pedimos a la IA el primer CRUD de Rockets sin reglas ni planes, solo iterando.

---

## Connections

- ¿Cuántas veces le has pedido algo a la IA y aceptaste lo primero que salió sin entender del todo cómo funcionaba?
- Cuando el resultado casi funciona, ¿vuelves a pedírselo al agente o lo arreglas tú a mano?

---

## Concepts

**Vibe Coding** — describes el resultado que quieres, dejas que el agente genere y avanzas guiándote por la sensación de "esto ya se parece a lo que buscaba".

**Short loop** — pedir, observar, corregir: cuanto más corto el lazo, más control conservas sobre la dirección antes de que el agente se aleje.

**Disposable baseline** — el primer resultado vale por velocidad, no por calidad; sirve para arrancar, no para confiar.

---

## Concrete practice

Producir un CRUD de Rockets en memoria, enchufado a la app que ya corre.

1. Modelo — `Create a Rocket model with id, name, seat capacity and operational range, kept in memory.`
2. Endpoints — `Add endpoints to create, list, read, update and delete rockets.`
3. Vista mínima — `Add a UI view that lists rockets and lets me create one.`
4. Checkpoint — corre la app, crea un rocket y compruébalo en la lista; acepta la primera versión que funcione de punta a punta.
5. Commit — `feat(rockets): scaffold CRUD via short vibe-coding loops`

---

## Conclusion

- Te dio un CRUD funcional en minutos; te costó estructura, validación y tests: solo sabes que "funciona en mi pantalla".
- ¿Podrías explicar qué generó el agente sin volver a leerlo línea a línea? ¿Confiarías ese código a otra persona del equipo?
- El lazo corto te dio velocidad pero poco control. El siguiente paso es nombrar y reutilizar lo que repites: prompts, rules y skills.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
