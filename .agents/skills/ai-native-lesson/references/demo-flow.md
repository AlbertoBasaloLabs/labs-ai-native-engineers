# From Vibe Coders to AI-Native Engineers — Demo commit log

Cada lección como un commit (Conventional Commits) sobre la demo **AstroBookings**.
El esqueleto ya existe (stack elegido, cero lógica funcional). El dominio se cubre en orden
`Rockets → Users → Launches → Bookings → Payments/refunds`, con el refactor estructural en
mitad de curso y lo transversal (logs, observability, errores) al final.

Formato: `tipo(scope): descripción de la demo`

---

## I — Human In The Loop

```
1.1  feat(rockets):      scaffold CRUD via short vibe-coding loops
1.2  chore(ai):          extract reusable prompt, rule and endpoint skill
1.3  feat(rockets):      add capacity & range validation via AI-DD flow
2.1  docs(context):      inventory skeleton, map signal vs noise
2.2  feat(users):        register operators and passengers
2.3  chore(rules):       define structure/naming rules, regen users
```

## II — Human On The Loop

```
3.1  docs(launches):     spec problem/solution/verification + lifecycle
3.2  docs(launches):     turn spec into verifiable task plan
3.3  feat(launches):     implement launches + state transitions from plan
4.1  test(bookings):     add e2e flow validating the booking spec
4.2  fix(bookings):      block overbooking against rocket capacity
4.3  refactor(bookings): apply early-review feedback on book + pay-mock
5.1  docs(legacy):       map implicit rules behind rockets/launches
5.2  docs(core):         triage result-pattern + central-log impact
5.3  refactor(core):     migrate dto→value-object w/ result, tests green
```

## III — Away From Keyboard

```
6.1  ci(hooks):          run lint+tests+quality-gate on each agent change
6.2  feat(payments):     operate pay/refund via mcp to mock gateway
6.3  chore(agents):      define tester, refactor and doc subagents
7.1  chore(obs):         slice logs/observability/errors into safe units
7.2  feat(app):          build api and webapp with parallel agents
7.3  feat(bookings):     orchestrate swarm for booking→payment flow
8.1  ci(loop):           turn build/test pipeline into self-correcting loop
8.2  feat(launches):     add stop-conditions + audit trail for cancel/suspend
8.3  feat(payments):     autonomous loop completes refunds, review AFK
```

---

## Cómo leer la trazabilidad por tipo de commit

- **Funcional** → `feat`, `fix` (rockets, users, launches, bookings, payments, app).
- **Calidad / verificación** → `test`, `refactor`.
- **No funcional** → `ci` (hooks, loop), `chore(obs)` (logs, observability, errores).
- **Propio del curso (método IA)** → `chore(ai|rules|agents)`, `docs(context|launches|legacy|core)`
  — prompts, reglas, skills, specs, subagentes, MCP.

## Nota de coherencia narrativa

Las únicas dos veces que aparece un commit "rojo" (`fix` / `refactor` correctivo) son **4.2**
(fallo provocado) y **5.3** (refactor estructural de mitad de curso). Es deliberado: el resto del
log debería ir casi todo en verde, lo que refuerza el mensaje de **adelantar el control**.

---

## Siguiente paso (pendiente de validar)

Añadir a cada commit su *body* (2–3 líneas) con:
- **Antes** — specs / tests / reglas que cargas antes de delegar.
- **Después** — qué entrega el agente y cómo se verifica.