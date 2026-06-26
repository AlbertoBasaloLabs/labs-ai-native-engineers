---
title: AI-Driven Development
description: Optimize the human-AI interaction.
url: 1-3-ai-driven-development
footer: AI-Driven Development · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.3 - AI-Driven Development

Con las primitives en la mano, añadimos a Rockets la validación de capacidad y rango, pero esta vez dirigiendo el lazo de forma deliberada.

---

## Connections

- Cuando el agente entrega, ¿revisas antes de pedir o pides y revisas al final?
- ¿Dónde pierdes más tiempo: explicando la tarea o corrigiendo el resultado?

---

## Concepts

**AI-Driven Development** — un flujo explícito: encuadrar, dejar generar, verificar y corregir; el humano dirige el lazo en vez de sufrirlo.

**Intent first** — describir el qué y el porqué (las reglas del dominio) antes del cómo reduce las idas y vueltas.

**Verify before accept** — definir cómo comprobarás el resultado *antes* de pedirlo convierte la revisión en algo objetivo.

---

## Concrete practice

Que Rockets rechace capacidad y rango inválidos, validado a través de un lazo AI-DD.

1. Encuadrar — `State the domain rules: seat capacity must be positive, operational range must stay within bounds.`
2. Generar con primitives — `Use the endpoint skill to add this validation to create and update rockets.`
3. Verificar — `List the checks you'll run, then test valid and invalid rockets against them.`
4. Corregir en lazo — devuelve el caso que falla y itera hasta que se sostenga.
5. Commit — `feat(rockets): add capacity & range validation via AI-DD flow`

---

## Conclusion

- Te dio validación fiable con menos reintentos a ciegas; te costó pensar antes el intent y la verificación.
- ¿Tu lazo ahora empieza por el resultado esperado o sigue empezando por el código?
- Dirigir bien el lazo exige alimentar el contexto correcto: el módulo 2 entra en Context Engineering.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
