# Course map — From Vibe Coders to AI-Native Engineers

Reference for placing any lesson in context. Read before drafting.

## The spine

The course follows one thread: **the human-AI loop lengthens and your intervention spreads out over time**. Three stages, eight modules, 24 lessons. Control is moved *earlier* — loaded into specs, tests and harness — so the agent delivers at the quality you would have demanded.

- **I — Human In The Loop** (you approve closely)
- **II — Human On The Loop** (you supervise)
- **III — Away From Keyboard** (you delegate)

## The 24 lessons

### I · Human In The Loop
**1 · Vibe Coding to AI-DD**
- 1.1 Vibe Coding — iterate in short loops until you get a result.
- 1.2 The AI coding Primitives — prompts, rules, skills: the base blocks.
- 1.3 AI-Driven Development — optimize the human-AI interaction.

**2 · Context Engineering**
- 2.1 The Context Window — how much fits, what's used, what's wasted.
- 2.2 Context Selection — prioritize what's relevant at each moment.
- 2.3 Deterministic rules — set rules to reduce randomness.

### II · Human On The Loop
**3 · Spec-Driven Development**
- 3.1 Specs as Source of Truth — problem, solution and verification in one contract.
- 3.2 From Spec to planned task — plan the implementation to satisfy the contract.
- 3.3 Writing code is the easy part — plans and rules to generate code and tests.

**4 · Trust but Verify**
- 4.1 E2E Behavior Validation — functional verification of the spec.
- 4.2 The fixing loop — from failure to fix and back to the test. **(RED moment)**
- 4.3 The review loop — early review for robust, maintainable code.

**5 · Legacy Refactoring**
- 5.1 Reading the Legacy — explore solutions and extract rules.
- 5.2 Change Triage — control and ease functional change.
- 5.3 Structural Refactoring — plan and document implementation changes. **(RED moment)**

### III · Away From Keyboard
**6 · Harness Engineering**
- 6.1 Hooks & Control Points — deterministic actions in the agent-model cycle.
- 6.2 MCP Integration — connect the agent to the project's real environment.
- 6.3 Subagents — roles, skills and configuration of secondary agents.

**7 · Agent Orchestration**
- 7.1 The Session Window Problem — split before drowning the context.
- 7.2 Sequential vs Parallel — coordination models and task sharing.
- 7.3 Context sharing — agent swarms with a common goal.

**8 · Loop Engineering**
- 8.1 From Pipelines to Loops — go back to fix or to do more.
- 8.2 Stop Conditions — the triage needed to know when to stop.
- 8.3 Away From Keyboard — trusting more requires checking more.

## The demo — AstroBookings

A space-travel booking system: a backend API + a frontend WebApp.

- **Rockets** have limited seat capacity and a specific operational range.
- **Launches** are scheduled by associating a rocket on a future date, with a price per seat and a minimum occupancy threshold.
- Launch lifecycle: `scheduled` → `confirmed` → `successful`; can go to `suspended` (low occupancy) or `canceled` (technical).
- **Users** are operators or passengers; register with email + name.
- **Operators** manage rockets and launches (cancellations, suspensions). **Passengers** book launches with available seats.
- **Payments and refunds** (from suspension/cancellation) go through a mock transactional gateway.
- Fictional, training-only; no security at the initial stage.

**Starting repo state:** front + back already runnable, with `GET /api/health` returning uptime, and the client calling and displaying it.

## Cross-cutting extras

Beyond the domain, the demo must also weave in transversal concerns and one structural refactor:
- Logs / observability, centralized error handling, helper libraries.
- At least one **structural refactoring** mid-course (a significant implementation change — e.g. DTO→Value Object, centralized logging, result pattern). This anchors lesson 5.3.

Introduce these as part of the method, not up front. Lesson 1.1 deliberately omits them to establish a raw baseline.

## Commit conventions

`type(scope): description`, three axes:
- Functional: `feat`, `fix`
- Quality: `test`, `refactor`, `ci`, `docs`, `chore`
- AI-course scopes: `ai`, `rules`, `agents`, `context`, `obs`, `hooks`, `loop`

Plus domain scopes for feature steps: `rockets`, `launches`, `bookings`, `payments`, `users`.

**Only two red commits in the whole course:** 4.2 (overbooking fix) and 5.3 (DTO→Value-Object refactor). Everything else is green. Keep the demo narratively coherent across all 24 commits.

## Authoritative plan

A full 24-lesson commit plan exists in Alberto's own files. When a lesson already has an assigned commit/body there, that wins. This skill provides the format and guardrails; confirm the increment with Alberto when in doubt rather than inventing domain steps that conflict with his plan.