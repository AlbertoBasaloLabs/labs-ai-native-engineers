---
title: Vibe Coding
description: Iterar en bucles cortos con la IA hasta obtener un resultado que funciona.
url: 1-1-vibe-coding
footer: Vibe Coding · &copy; [AlbertoBasalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy) 
marp: true
theme: ab
---

# 1.1 - Vibe Coding

Pedir, ejecutar y corregir en bucles cortos hasta que funcione.

> _Learn to code smarter._ 
> Por [Alberto Basalo](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)

---

## Connections

- ¿Cuántas veces has pedido algo a la IA, no era lo que querías, y has vuelto a intentarlo cambiando el prompt?
- ¿Sabrías repetir mañana el resultado que conseguiste hoy a golpe de impulso?

---

## Concepts

- **Vibe coding** 
  - Describes lo que quieres, ejecutas y corriges en bucles cortos hasta que funciona.

- **Loop corto** 
  - Cuanto antes ejecutas y observas, antes detectas la desviación y menos contexto se contamina.

- **El coste del impulso** 
  - Funciona, pero no es reproducible ni explicable: el conocimiento se queda en tu cabeza, no en el repo.

---

## Concrete practice

Generar un CRUD completo de `Rockets` por vibe coding, en bucles cortos.

---

- 1. Describe el recurso 
`Create a Rockets resource with id, name, seat capacity and operational range; expose CRUD endpoints over an in-memory store`
- 2. Ejecuta y prueba un endpoint 
`Run the app, create a rocket, then list rockets`
- 3. Corrige en un bucle corto 
`The list returns empty after creating a rocket; fix the in-memory store so it persists within the session`

---

- 4. Checkpoint: las cuatro operaciones del CRUD funcionan de extremo a extremo contra el store en memoria.
- 5. Commit 
`feat(rockets): scaffold CRUD via short vibe-coding loops`

---

## Conclusion

- Te dio velocidad: un CRUD entero en minutos sin escribir una línea.
- Te costó control: nada quedó escrito como regla ni es repetible.
- ¿Podrías recrear este resultado en otro recurso sin volver a improvisar? Eso es lo que extraeremos en la próxima lección.

> _Learn to code smarter._  
> [**Alberto Basalo**](https://albertobasalo.dev)@[AICode.Academy](https://aicode.academy)
