---
title: AI-Driven Development
description: El flujo Human In The Loop donde reglas y skills guían al agente y aparece la necesidad de specs.
url: 1-3-ai-driven-development
footer: AI-Driven Development · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.3 - AI-Driven Development

Cargar contexto, generar, revisar y corregir: un bucle deliberado con el humano dentro.

> _Learn to code smarter._ 
> Por [Alberto Basalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)

---

## Connections

- ¿Cuándo revisas lo que genera el agente: línea a línea, o solo cuando algo falla?
- ¿Qué pasa cuando la regla de negocio no está escrita en ninguna parte?

---

## Concepts

- **Human in the Loop**: 
  - Verificación en procesos cortos y repetibles
- **Rules over Tools**: 
  - Guiar con reglas y enseñar habilidades
- **Spec-Driven Development**: 
  - Explicar en detalle el problema y su verificación

---

## Concrete practice

Añadir validación de capacidad y rango a `Rockets` con el flujo AI-DD: el negocio escrito en una spec, cargada junto a reglas y skill.

---

- 1. Da un sitio al negocio 
`Write a short spec for Rockets: seat capacity must be a positive integer and operational range must fall within its allowed bounds`
- 2. Carga el contexto 
`Using the project-conventions rules and the Rockets spec, add validation to Rockets`
- 3. Genera y revisa en el bucle 
`Show the validation and the error response, then add the missing edge case for zero capacity`

---

- 4. Checkpoint: los rockets inválidos se rechazan con errores claros; los válidos siguen pasando.
- 5. Commit 
`feat(rockets): add capacity & range validation via AI-DD flow`

---

## Conclusion

- Te dio calidad sin perder control: revisas en cada vuelta y las reglas reducen las sorpresas.
- Te dio un sitio para el negocio: el *qué* del dominio ya no vive en tu cabeza ni en un prompt suelto.
- ¿Qué pertenece a las rules y qué a la spec?
- El próximo módulo ataca el contexto —qué cargar y qué descartar— para alimentar bien esas specs.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
