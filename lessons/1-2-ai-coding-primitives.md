---
title: The AI Coding Primitives
description: Prompts, rules and skills — the base blocks.
url: 1-2-ai-coding-primitives
footer: The AI Coding Primitives · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.2 - The AI Coding Primitives

El CRUD de Rockets ya corre, pero lo improvisamos. Hoy extraemos las piezas reutilizables que usaremos cada vez que toquemos un endpoint.

---

## Connections

- ¿Cuántas veces has reescrito casi el mismo prompt para tareas parecidas?
- ¿Has notado que el agente "olvida" tus preferencias entre una petición y la siguiente?

---

## Concepts

**Prompt** — instrucción puntual, de un solo uso, para una tarea concreta.

**Rule** — preferencia persistente que el agente aplica siempre, sin que la repitas.

**Skill** — procedimiento reutilizable y empaquetado: un cómo-hacer que invocas por su nombre.

---

## Concrete practice

Convertir lo improvisado en Rockets en un prompt reutilizable, una rule de proyecto y un skill de endpoint.

1. Capturar el prompt — `Save the CRUD prompt I used as a reusable, parameterized prompt.`
2. Definir una rule — `Write a project rule with my conventions: in-memory store and consistent endpoint naming.`
3. Empaquetar un skill — `Package the "create an endpoint" procedure as a named, reusable skill.`
4. Checkpoint — vuelve a generar un endpoint de Rockets con el skill y comprueba que sale igual con menos texto.
5. Commit — `chore(ai): extract reusable prompt, rule and endpoint skill`

---

## Conclusion

- Te dio reutilización y consistencia; te costó el tiempo de formalizar lo que antes improvisabas.
- ¿Qué parte de tu interacción con la IA sigue siendo improvisada y debería ser una pieza con nombre?
- Con piezas reutilizables, el siguiente paso es optimizar el flujo humano-IA completo: AI-Driven Development.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
