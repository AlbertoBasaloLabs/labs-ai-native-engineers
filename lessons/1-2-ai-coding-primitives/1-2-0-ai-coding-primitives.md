---
title: The AI Coding Primitives
description: Prompts, rules y skills, los bloques con los que se construye un flujo de trabajo con IA.
url: 1-2-ai-coding-primitives
footer: The AI Coding Primitives · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.2 - The AI Coding Primitives

Convertir el impulso en piezas reutilizables: prompts, rules y skills.

> _Learn to code smarter._ 
> Por [Alberto Basalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)

---

## Connections

- ¿Reescribes el mismo tipo de prompt una y otra vez para cada recurso nuevo?
- ¿Dónde viven hoy tus convenciones de proyecto: en tu cabeza o en un sitio que la IA pueda leer?

---

## Concepts

- **Prompt** 
  - Una instrucción reutilizable y parametrizable: el *qué*, listo para repetir.

- **Rules** 
  - Convenciones siempre activas que el agente respeta sin que las repitas: el *cómo*.

- **Skill** 
  - Un procedimiento empaquetado (prompt + reglas + pasos) para una tarea recurrente: el *qué* + el *cómo* + el *cuándo*.

---

## Concrete practice

Convertir el trabajo improvisado de 1.1 en tres primitivas reutilizables, sin cambiar el comportamiento de la app.

---

- 1. Extrae el prompt 
`From how we created Rockets, write a reusable prompt that scaffolds a CRUD resource given its name and fields`
- 2. Extrae las reglas 
`Capture the implicit conventions we followed (naming, folder layout, in-memory store) as always-on project rules`
- 3. Compón la skill 
`Combine the prompt and the rules into a skill that creates an endpoint resource end to end`

---

- 4. Checkpoint: vuelve a aplicar la skill sobre `Rockets`; mismo resultado, ahora reproducible.
- 5. Commit 
`chore(ai): extract reusable prompt, rule and endpoint skill`

---

## Conclusion

- Te dio reproducibilidad: el conocimiento salió de tu cabeza al repo.
- Te costó algo de formalización por adelantado.
- ¿Qué merece ser prompt, qué regla y qué skill?
- Tienes las piezas, pero aún las disparas a mano; la próxima lección las integra en un flujo de trabajo: el AI-DD.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
